---
layout: post
title: "How I prevented users registrations from disposable email addresses"
tags: dronesimulator
categories: web, backend
image: /assets/images/blog/2023-04-04-image.png
---

Recently one user of my web app dronesimulator.it ([here]({{ "/projects/dronesimulator.html" | relative_url }}) the article about that project) made many account registrations with lots of disposable email addresses so that he always had a fresh account to get around the usage limitations of the free tier.

He was really proud of his trick on he was making fun of the web app.

![The "suggested question" from the hackerman user]({{"/assets/images/blog/2023-04-04-suggested question.jpg" | relative_url }})

>This is a "suggested question" from that user, in which he says that he does not like the web app, but he get rid of the service limitations by registering many accounts


Thanks to him I discovered that dronesimulator needed an email domain verification procedure.

### What is a disposable email domain?

An email domain is called disposable when it easily allows to register unlimited new email addresses without any user verification.

Some examples of disposable email services are: temp-mail.org, 10minutesmail.com or guerrillamail.com.

### How do you check if an email address is disposable?

You can exploit some disposable domain checkers services that are available online such as:

- [This repo of disposable email domains](https://github.com/disposable-email-domains/disposable-email-domains) on GitHub that contains a list of disposable domains often updated
- [This free API from debounce.io](https://debounce.io/free-disposable-check-api/) that receives an email address and returns if it is considered disposable or not

### How do I implemented disposable check on new registrations?

My objective was to automate the domain verification process, but I also wanted to have control on the final valutation of each domain, in order to fix eventual false positive and, more frequently, false negatives.

In order to meet all of these requirements I created a new database table and adopted this verification flow:

```
Every time a new registration arrives check if the domain of the email address is already present in the table:

1. If it is already present, check the disposability of that domain according to table information

2. Else, if no record in the table for that domain is found:

    a. Query the free API service and get disposability info from there

    b. Create and store a record in the database table for that domain

    c. Returns the disposability information

```

By adopting a sort of "lookup table" on the disposability checker API, the results given by the check flow are verificable and updatable.

![Blocked domains table structure]({{"/assets/images/blog/2023-04-04-domains table.png" | relative_url }})

I noticed that the possibility to manually change the valutation of the domains is useful, in fact some disposable domains that were not considered disposable by the API were exploited to bypass this mechanism, but I fixed that by simply updating the relative table records.

### Conclusions

After the introduction of this functionality the percentage of fake / disposable email addresses adopted to register to dronesimulator decreased drastically and I almost never did have to manually intervene.


A couple of months after the introduction of this check, I received another particular "suggested question" from a "new" user:

![Happy ending for everyone]({{"/assets/images/blog/2023-04-04-new suggested question.png" | relative_url }})

The domain of the email address associated to his account was `@gmail.com` 😎👌🔥