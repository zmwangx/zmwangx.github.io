---
title: "We need an OS X security white paper"
date: 2015-10-03T03:34:24-07:00
date_display: October 3, 2015
---
Apple has been offering an excellent [iOS Security White Paper](https://www.apple.com/privacy/docs/iOS_Security_Guide.pdf) since at least 2012, and it's very informative. I highly encourage everyone to read it. It even explains some annoyances of iOS; for instance, [this week's Upgrade episode](http://www.relay.fm/upgrade/56) discussed, [in Gruber's words](https://daringfireball.net/linked/2015/10/01/upgrade-56), "the lousy, painstaking, and at times downright confusing experience of migrating to a new iOS device", and once you read the white paper you'll realize that many things just can't be migrated due to iOS's hardware security model — basically, certain classes of data are encrypted with crypto keys baked into the silicon (see the section "Hardware security features"). I'm not saying the migration experience should be this painful (I would love to see it fixed or improved), but at least there's an explanation.[^migration]

But I digress. This post is about OS X. I've been hunting for an OS X equivalent for a while now, but I don't think it exists. And recently people are talking about Apple's [updated Privacy website](https://www.apple.com/privacy/)[^site], so I went there with a glimmer of hope. End result: no luck. In fact, Apple links to its iOS Security White Paper at the bottom of "[Our Approach to Privacy](https://www.apple.com/privacy/approach-to-privacy)":

![iOS Security White Paper linked, but no OS X.](/img/20151003-ios-security-white-paper-but-no-osx.png)

But there's little to no mention of OS X (the words "Mac" and "OS X" each appears only once on the page). This is not surprising; OS X as the second class citizen is nothing new, and iPhones and Apple Watches are arguably more intimate, and hence more private devices — at least for most people. It is somewhat disappointing though.

I forgot to mention why I would like to see an OS X security white paper. The reason is simple: a lot of security features are under-explained. For instance, I might want to learn more about FileVault: why am I given the choice of decrypting my drive with iCloud — I believe it's not the case on iOS? How does iCloud handle my disk encryption key, if I allow it access (I don't)? Or I might want to learn more about System Integrity Protection: does it auto revert (or repair, in their eyes) some permissions (e.g., that of `/usr/local`), as I heard people talking about? Or maybe more about code signing and the inner workings of Gatekeeper: there's [recent news](http://arstechnica.com/security/2015/09/drop-dead-simple-exploit-completely-bypasses-macs-malware-gatekeeper/) of Gatekeeper workarounds. I guess some of these stuff can be found in Apple's support documents or developer documentation if you look hard enough, but it would be nice if the major security features and their implementations are presented coherently in a single document. Maybe the OS X security model is too complex and diverse to fit into a single document? I don't know. Anyway, I'll keep waiting.

[^migration]: Loss of certain classes of protected data (due to hardward crypto keys) during migration should in principle only apply to migration by "restoration". What about providing a direct phone-to-phone migration, where data could be decrypted and transferred on the fly? But that would at least require a lightning male to lightning male cable (or you would have to entrust your most sensitive data, which shouldn't even leave the phone under normal conditions, to your Wi-Fi, something Apple probably wouldn't do), and having to use a different, and actually unheard-of cable isn't very realistic, so it won't be happening any time soon.

[^site]: I haven't read through everything, but the idea of a [non-law-practicing-human readable privacy policy](https://www.apple.com/privacy/privacy-policy/) is great.