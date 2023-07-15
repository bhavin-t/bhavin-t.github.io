---
title: "linux from scratch"
date: 2023-07-15T14:23:47+01:00
draft: false
---
## :sparkles: intro
[linux from scratch (LFS)](https://www.linuxfromscratch.org/) has been on my radar for a very long time, and so at least 15 years after i first discovered it -- i'm giving it a go! 

for the uninitiated, linux from scratch is a step-by-step tutorial for building a linux distribution, entirely from source. i'll start with a functioning linux system, and mount a secondary drive to it, on which i'll format, partition, and bootstrap the actual lfs distribution.

--- 
## :confused_face: y tho
![y tho](https://i.kym-cdn.com/photos/images/newsfeed/001/255/097/022.jpg)

prior to this project the most involved linux install i ran through was arch linux in about 2008, and i learnt more about linux from this install than i have during any other project i've undertaken[^1].

so! my main goal for this project is to fill out my knowledge of linux and its internals EVEN MORE. i'm certainly not expecting to be able to roll a whole distro unassisted by the end of the project -- far from it -- but i do want to at least be able to know and understand all of the steps involved.

--- 

## :warning: complications

this project will be built on an m1 pro macbook pro. this poses an issue because the lfs book targets `x86`/`x86_64` architectures [^2], rather than the `arm64` architecture that apple silicon is based on. 

to that end -- i found the excellent [Linux From Scratch with Training Wheels](https://philsyme.net/lfs-tw/) which provides supplemental steps to enable lfs to be built for apple silicon :folded_hands: 

[^1]: i should be abundantly clear though: i hated the whole process. it took AT LEAST 5 failed attempts before i actually completed it successfully, and those attempts had to be spaced out so i didn't yeet my laptop out of the window.
[^2]: https://www.linuxfromscratch.org/lfs/view/stable/prologue/architecture.html

---

## :sparkles: the posts

with all of that said, here are my posts outlining my progress/thoughts of the process!:

1. coming soon!
2. ???