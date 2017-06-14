+++
date = "2017-06-08T12:00:00+01:00"
draft = false
title = "Blokada v2.0 roadmap"
author = "Karsen"

+++

It's been exciting several months for ad blocking on Android. When I started developing Blokada, it was just a side project of mine meant to test some less-known Android APIs and capabilities of the platform itself. At that time, the only existing ad blockers for Android were eating battery like crazy and slowing down device. Plus, they were quite cumbersome to use. I wanted to see if it's possible to build something that will block most of the ads across all apps, while being efficient and fast enough so that I won't notice it in terms of battery life, or network bandwidth speed or device performance.

It turns out, **it's totally possible**! And, people want it. During the relatively short life of Blokada so far, it's received a lot of very positive feedback, has gained a considerable userbase around the world, and is getting more and more popular every day. All of this is very encouraging for me to keep developing Blokada and simply making it the best ad blocker for Android.

So, if you use Blokada, **I'd like to thank you**, for your posts on Blokada's XDA thread, your reviews in the store, bug reports, new ideas, and hundreds of emails I've gotten in general. So, thank you! :)

As exciting as developing Blokada and seeing your overwhelmingly positive reactions is, it's also very time consuming, and I'm inevitably getting closer to the limit of my resources (in terms of time, money, skills and effort) I can contribute to this project. And since ordinary ways of supporting app development make little sense in this case (it's an ad blocker, after all), I've decided to do what you've been asking for for quite some time now, and open source Blokada.

So, **Blokada v2.0 is going to be fully open sourced**! To increase the chances of Blokada becoming a thriving open source project with fast development and numerous contributions (and not, erm, the other way around), I've been doing some preparations, and I'm close to finishing them. Here is the highlight of what's already done and what is going to happen next weeks.

### Refactoring

I've **rewritten most of the codebase** to transform it from a proof-of-concept, gimme-more-tape state to something that can be considered a bit more engineered, with the main goal of making it easy for potential contributors to jump in, quickly grasp the architecture, and make, well, contributions. This'll for sure cause some bugs to regress (show up again), but now there're unit tests to squish them for real.

### Translations

Blokada is a global phenomenon. I've been getting a lot of requests to get it translated to Spanish, German, Russian, French, Czech, and more. Heck, some of you even already offered help in translating it! This is really awesome. I had to do some work for Blokada to be 100% localisable, and now I'm proud to say that, **v2.0 will support translations**! I've set up a kick ass translation system that will make translating Blokada a breeze. If you are willing to help here, be on a lookout for the next post, that will describe the process in detail.

### Donations

As I said, developing an app of such quality takes a lot of time and effort, and while I was, and still am, committed to **making Blokada the best, most popular ad blocker for Android**, Blokada has grew bigger than just a side project of one guy. I'm sure open sourcing it is going to bring an influx of awesome contributions. However, every project needs core developers dedicated to doing some of the less exciting work, too. Since I'd love to have the possibility to focus on Blokada full-time, I'll be rolling out a donation system together with Blokada v2.0, so that people who find Blokada useful and wish for it to keep getting better, can make it happen.

I really hope this will work out, since this is the only way of funding I can think of that will allow for Blokada to stay independent and trustworthy, as any ad blocker should be. My ideal scenario here would be to have enough volume that'd allow to set up a budget for contributors to be rewarded for their involvement.

However, for this approach to succeed, Blokada v2.0 will need to grow its userbase even faster than now. So, if you are reading this, **you can help by promoting Blokada** on social networks, websites, blogs, forums, twitter - anywhere you can think of. Just a few words will contribute to increasing the awareness, installs, and ultimately, global penetration ( ͡° ͜ʖ ͡°).

### What's next

Mainly, I need some time to stabilize the new codebase. Blokada v2.0 probably won't be as stable as 1.2.x, which was actually really good, but the more bugs I eliminate now, the better. This also includes working on an API of Blokada, which I believe will come in handy in the future. Last but not least, I'll soon announce the translation system and ask for contributions, so that by the time v2.0 is ready, we get the translations in.

So, let's keep killing those ads... 😉
