---
layout: post
title:  making this website
date:   2021-05-12 11:10:16
description: meta, I know
---

The beauty of the web is there's room in it for everyone.

I've always liked the idea that my "place" could be a simple website where I could share a little bit about myself, my job, and whatever else.

For a long time, I used Squarespace to host a personal website. It got the job done alright. But the sites were slow and clunky. They're customizable, sort of. But it wasn't enough. I wanted a challenge — and more control. Control is everything.

So I finally got my shit together and made a website.

### The tools

I found this template on GitHub and forked the repo. It's called al-folio.

I wanted something with a blog functionality. Something like Wordpress felt like overkill given that I probably won't be posting here all that much. I like how this particular blog allows me to write entries in Markdown. Markdown is clean, simple and lightweight. (Plug: I wrote this post in a great macOS app called MacDown.)

All the code is stored in my forked GitHub repo, and I manage it from Visual Studio Code. From there, everything else is AWS.

I used to host my domain on Hover. But I knew I wanted to at least <em>try</em> to run everything through AWS. I wanted to teach myself how it all worked given that it's more or less the industry standard. AWS is also supremely integrated and, importantly for a newbie like me,  well-documented.

Sure, the scale at which I'm using AWS is microscopic. But I've learned a lot about it and I'm interested in checking out more services as I go.

### I'm mostly using Amplify, Route 53 and S3

I stumbled upon Amplify almost accidentally.

The GitHub repo I forked is powered by Jekyll, and one of the big selling points was how easily one could deploy on GitHub Pages. However, because I was ride-or-die AWS, I started searching for a similar kind of plug-and-play deployment option through AWS. Lo and behold, Amplify did exactly that.

All I had to do was link up my forked repo's master branch to Amplify, make a few clicks, and the site was live.

### But what about that slick custom domain?

Here's where Route 53 entered the fold.

A few months ago, I did the yeoman's work of swapping the registration from Hover to Route 53, which is the AWS Domain Name System (DNS) service. The process was a bit of a pain. But it paid off when the time came to deploy the Amplify app. The tight integrations across services meant it was an extra couple clicks to have the site up and running at my personal domain.

I'm hoping to figure out how to use S3 image urls in blog posts like this one. Right now I have to store them locally. But that's the S3 explanation.

### The bottom line

The website is up. I'm pleased. Compared to, say, Squarespace's business plan ($18/month), my total AWS bill is about $5/month.

And the personal growth? Priceless.