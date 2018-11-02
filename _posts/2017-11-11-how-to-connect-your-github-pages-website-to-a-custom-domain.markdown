---
layout:     post
title:      "How to connect your Github Pages website to a custom domain"
date:       2017-11-11 07:55:00 +1300
categories: connect github pages website custom domain
---

This tutorial will teach you how to connect your Github Pages website to a custom domain
----------------------------------------------------------------------------------------

1.  Register a custom domain. If you don't have one yet, you can use [Freenom](http://www.freenom.com/en/index.html?lang=en) to get a free one.
2.  In Github navigate to the repository you wish to connect to the custom domain.
3.  Ensure The Setting _source Is Set To master_ or _/docs and press the save button_
4.  The settings for choosing a custom domain will now be shown. Type the domain which you would like to use. I'd go with something like _www.example.com_ or _subdomain.example.com_
5.  Press save.
6.  Now is the time to connect your domain to a DNS proxy such as [Cloudflare](https://www.cloudflare.com/).
7.  In your domain's DNS settings, configure the following item.

|Type |Name|Value             |
|:----|:---|:-----------------|
|CNAME|www |USERNAME.github.io|

1.  If you're using a subdomain (for example subdomain.example.com) change _www_ to the subdomain you chose.
2.  Also, replace _USERNAME_ with the Github username of the repository owner.

> This page was imported from the old blog with little to no modifications
