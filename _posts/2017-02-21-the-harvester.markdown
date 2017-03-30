---
layout: post
title:  "The Harvester"
date:   2017-03-29 11:24:00 +0530
categories: Pentest, footprinting, reconnaissance
author: "Gabriela"
---

Hi folks! 

Today I will talk about a tool for reconnaissance, The Harvester. 
This tool catalogues emails, subdomains, hosts, employee names, open ports.
I uses public sources such as search engines, PGP key servers and SHODAN computer database.
This tool was created by [Christian Martorella][cm-github].

This tool allows you to make passive and active discovery. The passive siscovery involves the search engines like google, bing, some social networks like linkedin and shodan search engine that search for ports and bunners if hosts available.
The active discovery involves DNS brute force, DNS reverse lookup and DNS TDL expasion. 

The parameters available are:
{% highlight %}
-d to define the target
-b: defines the data source like baidu, bing, bingapi, dogpile,google, googleCSE, googleplus, google-profiles, linkedin, pgp, twitter, vhost, yahoo or all
-s: defines a start for the result
-v: Verify host name via dns resolution and search for virtual hosts
-f: Save the results into an HTML and XML file (both)
-n: Perform a DNS reverse query on all ranges discovered
-c: Perform a DNS brute force for the domain name
-t: Perform a DNS TLD expansion discovery
-e: Use this DNS server
-l: Limit the number of results to work with(bing goes from 50 to 50 results,
    google 100 to 100, and pgp doesn't use this option)
-h: use SHODAN database to query discovered hosts
{% endhighlight %}

That's it!



[cm-github]: https://github.com/laramies
 
