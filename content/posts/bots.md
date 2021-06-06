---
title: "Learning Splunk Through BOTS"
date: 2021-04-30T13:48:47-04:00
draft: false
---

On May 14th, I participated in Splunk's BOTS CTF for the first time and it was a ton of fun! I created a team with someone I met in the [BHIS Getting Started in Security](https://wildwesthackinfest.com/antisyphon/getting-started-in-security-with-bhis-and-mitre-attck-john-strand/) Discord. Neither of us had production experience with Splunk, and we came in 56 out of 209 teams. Though I can't write in too much detail about the challenges since this version of BOTS is still running, here are some resources I used to prepare.

![BOTSv5 Score](/images/bots-score.png)

## Accessing Prior Datasets 

My exposure to Splunk prior to this was through completing challenges from previous versions on BOTS. The current version is v5, but Splunk [releases older verisons](https://www.splunk.com/en_us/blog/security/botsv3-dataset-released.html) after they've finished running them. To date, versions 1-3 have been released.  

Released versions can be found on Splunk's Github. The questions, answers, and hints are not part of this download unfortunately. For that, you'll have to email bots@splunk.com, and they'll reply with a download link. They responded to my inquiry in less than 24 hours.

![Email bots at spunk](/images/bots-email.png)

Each version of BOTS has utilized different data Sourcetypes and Add-Ons, so each repo's README has relevant instructions for configuring Splunk appropriately. 
- https://github.com/splunk/botsv3
- https://github.com/splunk/botsv2
- https://github.com/splunk/botsv1

Splunk has also open sourced their [scoreboard app](https://github.com/splunk/SA-ctf_scoreboard) if you're interested in running that to get an authentic experience. Personally, I just ran with the provided csv files. 

## BOTS Walkthroughs

I had success running both the v2 and v3 datasets in a single instance. I opted to run it in a Debian 10 virtual machine with KVM. 

I first worked through the BOTSv3 dataset which provided a good introduction. After a while, I was hitting some roadblocks in my understanding, so I switched to working through some of the easier challenges in v2. Shortly thereafter, I found [this app](https://splunkbase.splunk.com/app/4430/), which provided a nice guide for the APT scenario in BOTSv2. This helped improve my overall understanding of Splunk and gave me some ideas on how to approach questions I missed in v3. 

There's also [this](https://www.youtube.com/watch?v=RXDbir6B5mE) fantastic walkthrough on v3.
