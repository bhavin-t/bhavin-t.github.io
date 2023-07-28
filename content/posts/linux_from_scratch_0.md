+++ 
draft = true
date = 2023-07-16T13:00:07+01:00
title = "linux from scratch, part 0"
description = ""
slug = ""
authors = ["bhavin"]
tags = ["lfs"]
categories = ["lfs"]
externalLink = ""
series = ["linux from scratch"]
+++

## :green_book: it begins... ish

before even opening the lfs book and starting to get stuck in, my first decision was to figure out which book to even use. the lfs project has two variants -- [one that covers a systemd flavoured setup](https://www.linuxfromscratch.org/lfs/view/stable-systemd/), and [the other for a sysvinit flavoured one](https://www.linuxfromscratch.org/lfs/view/stable/). 

i would ***love*** to tell you with confidence the ins-and-outs of both of them, but the truth is, i don't know. so i did the thing any reasonable engineer would do and went onto reddit. it didn't take long for me to realise that people really, *really* hated systemd...


> SystemD is a cancer
> — <cite>UnicornMolestor</cite>

mildly amused by this, i googled it a bit more and it turns out [there are a bunch](https://ihatesystemd.com/)[ of different sites about it](https://nosystemd.org/). i spent a few minutes reading those sites and ultimately, and possibly to the website author's dismay -- i still remain unconvinced either way of the good or bad of systemd.

when i got out of that rabbithole, i found this, significantly more useful, reddit comment breaking down the differences (at least in the context of lfs) between the two:

> Non-systemd uses a more classical, shell script-based approach to init, where all the init files are just shell scripts that get called in sequence based on symlinks, etc. Very simple and easy to understand what's going on, very bare-bones and minimal. Not very flexible though, but you probably don't care about that on LFS. Systemd on the other hand is a more complex init system that does a lot more and is way more flexible, which also makes it harder to set up correctly and can be more confusing especially if you are unfamiliar with how the init process works just overall.
> — <cite>leadbasedtoy [^1]</cite>

though i heed the warning of systemd being a more complex system (and by extension increasing significantly the number of times i'm likely to ragequit during this project), the fact that most major linux distros (Debian, Fedora, CentOS, Red Hat, Ubuntu, OpenSUSE, Arch) use systemd is enough to convince me to choose the systemd version of lfs. **overall i think that it would be most beneficial for me to learn how modern linux systems are architected, and if that is systemd -- then so be it.**

SO. now that that's settled, it's time to dive in!


[^1]: https://www.reddit.com/r/linuxfromscratch/comments/gae6dg/systemd_vs_nonsystemd/fozfeup/