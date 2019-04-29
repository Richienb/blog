---
layout:     post
title:      "How to connect your GitHub Pages website to a custom domain"
date:       2017-11-11 07:55:00 +1300
categories: connect github pages website custom domain
---

This tutorial will teach you how to connect your GitHub Pages website to a custom domain

1.  Register a custom domain. If you don't have one yet, you can use [Freenom](http://www.freenom.com/en/index.html?lang=en) to get a free one.
2.  In Github navigate to the repository you wish to connect to the custom domain.
3.  Ensure the setting *source* is selected to something other than *none* and press the *save button*.
4.  Below the *source* selector, type the domain which you would like to use. I'd go with something like _www.example.com_ or _subdomain.example.com_
5.  Press save.
6.  Now is the time to connect your domain to a DNS proxy such as [Cloudflare](https://www.cloudflare.com/), if you wish.
7.  In your domain's DNS settings, configure the following item.

|Type |Name|Value             |
|:----|:---|:-----------------|
|CNAME|www |USERNAME.github.io|
|A    |@   |185.199.108.153   |
|A    |@   |185.199.109.153   |
|A    |@   |185.199.110.153   |
|A    |@   |185.199.111.153   |

1.  If you're using a subdomain (for example subdomain.example.com) change *www* to the subdomain you want.
2.  Remember to replace *USERNAME* with the GitHub username of the repository owner.

> This page was imported from the old blog with little modification.
