---
title: What will AI do to our brains when it gets too good?
description: We learn a lot from struggling to understand. What will happen when AI removes the struggle?
slug: what-will-happen-to-our-brains-when-ai-gets-good
date: 2026-07-24 00:00:00+0000
# categories:
#     - Projects
# tags:
#     - Software Development
---

I think Claude may have just saved me 200 hours of debugging and banging my head against the keyboard.

First off, some context. When I was in college in 2015 I worked for the school's IT department where I was tasked with deploying a Shibboleth SSO server for the whole university. I suspect the administration just wanted to get me off their backs because when I was given the assignment my supervisor said "good luck, nobody has been able to figure this out". It took me 4 months. At between 10 and 15 hours a week that comes out to about 200 hours I spent trying to figure out how to go from 0 to understanding how to deploy complicated enterprise software. In the end, I prevailed and walked away from the experience with a deep understanding of Java server apps, Docker, Linux and a whole toolbox of troubleshooting tools that have served me well for the past 10 years.

Today I faced a similarly sticky problem. The Safari web extension for Digital Carrot wasn't getting recognized by Safari. I had no leads, no idea where to start and no understanding of the MacOS code signing and notarization system. I could have easily spent 200 hours shooting blanks like I did in 2015, but this time around I had Claude. My first session was a mess. Claude went down a completely wrong path and tried to convince me to turn off "Automatic Code Signing" in xCode, which would have been a disaster. This did give me the idea that my issues might be related to code signing.

During my second session, Claude recognized a few issues in my configuration, and helped me fix them, but wasn't able to resolve the issue. I was able to go through the commands that Claude was using and independently verify that the issue was indeed related to code signing. This gave me enough of an understanding to do my own investigation.

During my third session I was able to give Claude the right information it needed and it was able to just fix the problem with the app in about 15 minutes. As it turned out, the VM I was testing the app on wasn't proactively pulling the app notarization from Apple's servers, and stapling the notarization to the app as well as the DMG fixed the problem.

This experience left me feeling conflicted. For one, I don't really understand what "stapling the notarization to the app as well as the DMG fixed the problem" really means. I get the gist of it, but ultimately I don't have a much better understanding of Apple's code signing infrastructure than I did yesterday. I may have saved 200 hours, but what I didn't gain was very much knowledge. That said it wasn't all fruitless. I now have some useful tools in my tool belt that can help me diagnose these kinds of issues in the future.

All of this makes me wonder if we are in somewhat of a sweet spot intellectually speaking with regards to the current state of AI. AI is smart enough to be able to legitimately save us a lot of time. It's also dumb enough that we still have to contribute something to the party. If Claude had just figured out the issue during my first session I would have learned next to nothing. What will happen to us on a cognitive level when we ultimately get to that point?
