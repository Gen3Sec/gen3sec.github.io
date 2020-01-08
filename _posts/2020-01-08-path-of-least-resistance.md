---
layout: post
title:  "Path of Least Resistance"
author: gen3sec
categories: [ infosec, passwords, business_enablement, polr ]
image: assets/images/computer-problem.png
featured: true
---

# Path of Least Resistance

## Frustration of a Security Leader

I try to be calm and level-headed; however, I am not immune to the shared frustrations of the security community when end users are not compliant with the controls we implement. 

When exploring new controls, I try to find the least invasive option that reduces friction and promotes productivity to the greatest extent possible. 

I know - definitively - if the controls are in the least bit disruptive, like water going around a large rock, users will find a way to bypass them. My users know I am fanatical about avoiding this, as well. My goal is to securely enable them to complete their work and promote engagement with the security team to find best practices.

With this in mind, this morning __I was the user__ that was sucked in to the vortex of security hell doing my absolute best to not become water looking for a way around the rock. 

## Passwords, really!?

I know. There has been pervasive railing against passwords lately, but my most recent experience has led me to create this as the first post on this shiny new blog.

To be fair, there has been a considerable amount of improvement over the last couple of years with password use in effort to improve hygiene; however, we have a long way to go. 

This morning, I received an alert from a government-based website warning me my password would expire in the next 30 days. Ironically, they are not following their own recommendations by [NIST 800-63B](https://pages.nist.gov/800-63-3/sp800-63b.html), some highlights: 

    - utilize a passphrase 12+ characters
    - eliminate required complexity
    - remove expiration of password unless there is an Indication of Compromise (IOC)

My password for that site met their previously defined minimum characteristics, including minimum of 12-characters, complexity requirements of upper and lower case, number and symbol. Oh but wait! It can't have some symbols - more on this later. There was no indication of compromise for the password on my account, so there should not have been a requirement to update.

## Password Managers

I have been a huge fan and promote the use of password managers religiously. They help drastically reduce the overhead of using passwords.

Of course, there are some apparent concerns, like the compromise of the master password/passphrase. Most solutions do a good job of forcing multi-factor authentication when adding a new device minimizing that risk, though. 

Password reuse is still an issue from what I have observed, likely due to integration weaknesses or streamlined experiences for some sites. Overall, I believe is has helped in this area, as well. 

I have absolutely seen a reduction in sticky note utilization both physically and digitally by implementing a password manager.

## My Experience

![Photo by Matthew Brodeur on Unsplash](https://github.com/Gen3Sec/gen3sec.github.io/blob/master/assets/images/password.jpg)"")

With all of that, let's explore my experience from this morning. 

NOTICE: You have 30 days to update your password! 

_Me_: Ok, fine. Let's go ahead and get this done so I can clear the notification out of my inbox. 

I log in. Ok, where do I go to update my password? 4 menus later, I find it. Phew.

_Site_: Enter your current password. 

_Me_: Umm ok. I just signed in, passed MFA, and you have a auto-timeout of a couple of minutes, but fine with the password manager, it's a couple of clicks. 

_Site_: Enter your new password, it must be 12 - 25-characters, have upper and lower case, include a number, and at least one special character. 

_Me_: Ok, should be easy enough, fire up the password manager's password generator, select max characters, include all complexity (which is default), copy password, paste it both fields, click update.

_Password manager_: want to save this?

_Me_: Umm yes, no way I am remembering that ridiculous string.

_Password manager_: ok cool, I got it.

_Site_: Wait! Hold on there "Turbo", you can have _those_ special characters! 

Ok. I get it cross-site scripting, SQL-injection, yada yada, but ugh. Fine, I'll generate a new password without special characters and through a "good" special character in somewhere randomly.

_Site_: Sounds good, enter current password.

_Me_: Hey password manager, do this.

_PM_: I only have your new, denied current password.

_Me_: [Losing patience rapidly] Ok. Opens desktop version of PM, looks up site, opens history, copies old ridiculous password (I think).

Paste "old, old" password. Generate new password without special characters, throw in SC randomly, happens to be toward the end of the mega long string. Copy/paste x2.

_Site_: No! You MUST have a special character!

_Me_: Umm, thought I did!? Checks. Yep, I did!? 

_Site_: No, you didn't. You MUST have a special character!

_Me_: Ok. I'll try again. Repeat previous process in its entirety wondering if I really need access to this site.

_Site_: NO! You MUST have a special character! 

_Me_: Oh! So, you force a ridiculous password but truncate everything after 8-characters. Fine, I will create **another** password and put the SC in the first 8-characters. 

_Site_: That's cute, but your current password is incorrect.

_Me_: ... I wonder what the strength of the window is next to me and if the laptop will go through it?!

After copying/pasting 3 or 4 previous passwords, plus the new password x2 each time, I finally achieved Nirvana:

_Site_: Success, you have updated your password! Would you like to sign-in?

_Me_: Absolutely NOT. I really hope I saved the new password into the password manager. 

## Enable Good Behavior

We **must** find a way to promote good behavior. Especially, now that Identity and Access Management (IAM) is becoming the "new perimeter", we have to figure out how to help users improve password hygiene. I thought the update NIST recommendations would be a helpful push but with mind-numbingly-slow adoption, we have to figure out something else. Let's not even broach the topic of compliance. HIPAA likely won't adopt NISTs recommendations for the next few decades, leaving organizations fearful of implementing them and not being able to check-a-box for compliance. 

> Sadly,"P@ssw0rd#123!" or "Winter2020!!" would have worked just fine and taken me 30 seconds. In fact, probably 80% of the passwords you see on the "Top Bad Passwords" lists floating around would have sufficed. Then, my next forced update would have landed perfectly in Spring. I guess, at least, I would have been compliant! 

I do think biometric, while young and not thoroughly tested, shows a lot of promise. Obvious fears come into play with biometrics, though and I'm not sure that is the best answer. _Update_ [maybe not](https://www.securitysales.com/news/united-states-worst-biometric-data/).

NIST's updated recommendations in combination with password managers has a lot of promise, everyone just needs to get on-board. I think this is the best solution until we find a viable password-free option.

## Path of Least Resistance

I almost named this blog "Path of Least Resistance" or "POLR" but one is too long and the other non-sensical. 

It is my passion to discover ways to provide the path of least resistance as the secure path for users and make security something that they don't have to think about, but something that just happens.

One day, we will get there. Hopefully. Until then, I hope you will join me and partner with your users and become their advocate on best practices in dealing with the big-arse rock in their way and not **being** the rock.

_UPDATE_: Since creating the post a couple of days ago and going through the editing process, I have tried to access that site again. Guess what!? Yep. "We're sorry, your password is invalid" (which someone should update the verbiage on that - now I know I can password spray other accounts when finding a username that works). Here we go again...