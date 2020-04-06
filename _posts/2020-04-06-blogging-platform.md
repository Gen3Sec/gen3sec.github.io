---
layout: post
title: Blogging platform
author: Gen3Sec
categories:
- blogging
image: ''
featured: false

---
# Blogging

There are obviously a variety of blogging platforms from which to choose.

## WordPress

WordPress is the historical front-runner, and for good reason. They make blogging dead simple. They have both free and paid versions. I have historically use both free and paid versions. While they work well, security is an ever-present issue on WordPress. In addition, I want to use my own domain name, yet I am not consistent in blogging enough to use the paid version.

There are a considerable amount of options to WordPress. I have looked at a few of them, but none seemed as viable as WP for whatever reason. Either they weren't as feature-rich, they were overly complex to use, on and on.

## GitHub Pages

I finally bumped into GitHub Pages. GitHub offers a free static site for your repository.

You simply create a free GitHub account. Create a repository, name it what you want your site to be, e.g. gen3sec.github.io and viola, you can install a theme and get to work. If you want to use your own domain, it is very simple. Change your DNS to GitHub requirements, got into settings in your repository, add your custom domain, e.g. gen3sec.io and even click on https for enhance security. All the magic happens in the background. No installing certs, etc.

There are a massive amount of Jekyll themes that plug-and-play similar to installing a theme for WordPress. You can browse for [themes](https://jekyllthemes.io/) just like you would for WordPress, download the .zip file from the proper GitHub repository, move it to your GitHub repo folder and push it up. Your site is set-up and ready-to-go!

> Stay tuned for a full write-up on setting up a GitHub Pages site coming soon.

I enjoyed using GitHub Pages, writing in Visual Studios Code editor, and pushing my post up just like I would do for a code commit. It made the blogging experience simple, efficient, and free!

GitHub Pages uses Ruby Gems to add functionality to your blog like RSS feeds and a host of other features providing a feature-rich environment similar to WordPress. You can use Google Analytics, Disqus for comments, and most things like you would on a normal blogging platform.

There is a slight technical requirement to using GitHub Pages, but it is not overwhelming. Just don't make it harder than it needs to be. Configuration and a few other things are completed using YAML, which is essentially key: attribute (e.g. Author: Gen3Sec). Spacing matters in YAML, but again it isn't overly technical and very easy to learn.

Then, just about the time you get frightened away by the technical necessities, apps like [Forestry](https://app.forestry.io/) step in and give you a free WYSIWYG front end where you can write a post almost exactly like you would in WordPress making the process crazy simple.

All in all, GitHub Pages is a fantastic blogging platform and fits all of my needs perfectly. I suspect it would fit the majority use-cases. I would at least check it out before spending money on a different platform. 

I will do a step-by-step write-up and standing-it-up as soon as I can. If you have questions before then, drop them in the comments. I'm happy to help if you are interested. 