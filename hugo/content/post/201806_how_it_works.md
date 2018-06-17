+++
date = "2018-06-17T08:00:00+01:00"
draft = false
title = "How does Blokada work?"
author = "Sebastian"

+++

_This article is brought to you by Sebastian, one of Blokada Insiders, and is the first in a series of articles aiming to improve your understanding of ad blocking, privacy and malware protection, and related topics._

### In very simple words, how does Blokada work and what is that VPN?

We all know that blocking ads is certainly something we all want. While some developers in fact rely on the revenue coming from displaying ads on their apps, the majority of ads we want to block are annoying, they increase the amount of traffic and simply ruin user experience, to put it straightforward (_personal advice: if you use an app whose developers seems to really depend on ad revenue, you can whitelist that app on Blokada, and URL requests from that app won't be filtered_).

There are several solutions to block ads available at the moment, but most of them are somewhat complex on the field of privacy data, others require special measures like rooting your phone, and others block ads on webpages but the rest of the system still displays ads. Nevertheless, Blokada requires none of this measures, and blocks not only webpages but also apps. Let’s see in short terms how Blokada does it.

### So, how does Blokada work?

To put it simply, Blokada generates a Virtual Private Network, a VPN, on your phone, and through the use of that VPN it filters traffic against hosts lists that contain hosts that are known as ad hosts. Also, it provides alternate DNS, so eventually that traffic will be resolved with the use of those DNS.

Basically two parts: first through the use a VPN all traffic is checked against a host list that contain ad delivery hosts; the second part is the host list itself, which is automatically updated within Blokada from known hosts list (like AdZHosts). A third component is the alternate DNS option provided by Blokada, but we’re not going to get into it now.

_To get things clear, DNS stands for “Domain Name Server” and/or Domain Name System, and while it’s much more complex than these few words, for the purpose of this short article we’re going to say that it is the system by which an URL is converted to an IP address, or, how your phone finally knows which IP is www.google.com. Blokada allows to use other DNS different from the system DNS, but by default the DNS used is the system DNS._

## Now, what is a VPN and how does the Blokada VPN affect the privacy of my data?

A lot of people have asked about the privacy of their data, since Android will always tell you that there is an active VPN on your phone when Blokada is activated. In short words, a VPN is a method that allows, among many other things, for re-routing traffic. When Blokada is activated, traffic is routed locally on your phone and passed through the hosts lists.

If there is a match between the URL that a webpage or an app tries to reach and an entry on the host list (the one that contain the ads hosts), then that connection is blocked. If there's no match, then the data is retrieved from the host and delivered to your phone, be it a webpage or an app.

![Ad blocking diagram](/img/howitworks_1.png)

## Does the Blokada VPN mean that my data is passing through third party hands?

No. The Blokada VPN is a local VPN and its reason is to route all the traffic through the hosts filters to know when a requested URL matches an ad host. As it was said before, if there’s an URL request to a host on the hosts lists, the request is blocked, so the ad isn’t even reaching the phone (this is where Blokada also helps in saving data, because it blocks the ad from the very request of it, not just displaying it). No data is passing through third party servers or hands or screens nor it is stored anywhere.

So, for the peace of your mind, using Blokada and seeing that VPN android alert doesn't mean your data is at risk. This method is the reason why Blokada works not only for webpages and inside a specific browser like any other browser extension, but also on any other app on your Android system that requests an URL.

## Technical notes!

When we are trying to explain in simple words something that has several technical aspects, there always has to be a section with the correct terms, specially for readers with advanced knowledge. In this article we made a few compromises to keep it simple, but there are two important things.

1. The first one: we used the concept of "URL request" to explain how ads are delivered, but Blokada in fact works at DNS level, meaning it filters not by URL but by domain. At DNS level, a domain is associated with an IP, and Blokada works at this level. These concepts -the DNS system- are a little bit technical since the DNS system involves "levels" among other things (the server that knows where to find .com domains knows where are the next layer of DNS, so it asks for a given .com domain to that DNS server, it's a recursive query). For the purpose of this article we let it at "URL request", but in reality Blokada works with domains, as in the DNS system (in the DNS system there's no such concept as URL, but domain). We took the liberty to explain it with the use of the term URL since it is far more known than the concepts around the DNS system.

2. The second one: there are two kind of hosts lists. The common ones, those used by Blokada, are composed by a domain and its associated IP address -and if there’s a match between the requested domain and an entry on the list, then the domain is blocked-. The other ones, commonly known as “cosmetic filtering” are used by some other ad blockers, and have another function. The difference is the following: when an ad is blocked, the webpage itself -or app itself- doesn't know that the ad has been blocked, it simply doesn't display it. Sometimes the consequence of this is a white space or some other layout issue, since the webpage or app had a space on the layout reserved for that ad. These other ad blockers sometimes use what is known as "cosmetic filtering", meaning it filters content according to some other rules (like CSS styling, by detecting on the CSS where are ads located on the webpage) and work on the layout of the webpage. Blokada doesn’t work on this type of filtering, since Blokada works at domain level.
