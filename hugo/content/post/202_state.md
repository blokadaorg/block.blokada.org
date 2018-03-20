+++
date = "2017-07-31T13:00:00+01:00"
draft = false
title = "A state of Blokada v2.0"
author = "Karol"

+++

It's been a week since Blokada ad blocker is open sourced and available for free. Here is a short summary of the improvements introduced between versions 2.0 and 2.0.2.

I got great feedback from the XDA folks as usual, and I've been addressing reported problems as they come. The biggest issue was the stability around imminent network connectivity changes. Apparently, connectivity state events sent by the OS cannot always be trusted, so I introduced some mechanisms (including a watchdog) to make Blokada more aware of the actual state, while not killing the battery. I fixed a bunch of bugs on the way too, so v2.0.2 should really be more snappy.

There was also a problem with dropping filters (hosts count 0), and in result, not blocking any ads, which I also addressed.

In the meantime, we've got full German and Dutch translations, so I'm releasing them as well :).

so, after we let the new version sink in and confirm it's stable, the long-awaited app whitelisting feature is next on the todo list :)

Enjoy!
