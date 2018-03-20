+++
date = "2017-08-17T13:00:00+01:00"
draft = false
title = "How to whitelist apps in Blokada"
author = "Karol"

+++

Blokada 2.1 introduced a long-awaited app whitelisting feature. This is very useful for dealing with apps that do not work correctly with ad blocking. Some apps, like Google Play Store or GMail are whitelisted out of the box. As always, you have full control how Blokada ad blocker works, so you can easily add and delete whitelisted apps.

Here is a video that demonstrates app whitelisting with XDA Labs app, which used to have problems with downloading apps if Blokada was on. Not anymore!

<div class="yt-container"><iframe class="yt-video" src="https://www.youtube.com/embed/xIKsSWTxAow?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe></div>

To add an app, go to the whitelist section, tap the add button, and simply start typing either app's name or package name (application ID). Blokada will show you suggestions as you type. Once you select and confirm the app, it'll show up in the whitelist. Blokada will also reactivate itself since it's required for the changes to take effect.

Keep in mind a few things while using this feature in it's early release:

- Not every app will immediately act properly after being whitelisted. In some rare cases you may need to kill and restart that app.
- App whitelisting is only supported by the optimised blocking mechanism (at least in 2.1). If you are using standard blocking, you'll see a message telling you app whitelisting is ignored.
- Some apps will be whitelisted by default if you just installed Blokada. In case you're updating from earlier version, they may not show up, in order to not mess with your custom filters you may have added. Simply add any apps you want to whitelist as you go. Alternatively, if you really want to have the "factory" filters configuration, simply delete all of them (both from the whitelist and the blacklist), then restart Blokada. The defaults will show up.

Enjoy!
