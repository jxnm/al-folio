---
layout: post
title:  making this website
date:   2021-05-14 10:01:16
description: meta, I know
---

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}/assets/img/0513_tree-bud.jpg">
    </div>
</div>
<div class="caption">
    The start of something new. (<a href="https://unsplash.com/photos/nrsgYdyJJxs">Unsplash</a>)
</div>

The beauty of the web is there's room in it for everyone.

I've always liked the idea that my "place" could be a simple website where I could share a little bit about myself, my job, and whatever else.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}/assets/img/0514_creedthoughts.jpg">
    </div>
</div>
<div class="caption">
    OK, hopefully not like <em>this</em>. (<a href="https://www.youtube.com/watch?v=1e5td7-Bpvc">YouTube</a>)
</div>

For a long time, I used Squarespace to host a personal website. It got the job done alright. But the sites were slow and clunky. They're customizable, sort of. But it wasn't enough. I wanted a challenge — and more control. Control is everything.

So I finally got my shit together and made a website.

### The tools

I found this template on GitHub and forked the repo. It's called <a href="https://github.com/alshedivat/al-folio">al-folio</a>.

I wanted something with a clean and simple look, plus a blog functionality. A proper CMS like Wordpress felt like overkill given that I probably won't be posting here all that much. I like how this particular blog allows me to write entries in Markdown, which is super simple and lightweight. (Plug: I use a great open-source macOS app called <a href="https://macdown.uranusjr.com">MacDown</a>.)

All the code is stored in my forked GitHub repo, which I push changes to via Visual Studio Code. From there, everything else is AWS.

I used to host my domain on Hover. But I knew I wanted to at least <em>try</em> to run everything through AWS. I wanted to teach myself how it all worked given that it's more or less the industry standard. AWS is also supremely integrated and, importantly for a newbie like me,  well-documented.

The scale at which I'm using AWS is microscopic. But I've learned a lot about it and I'm interested in checking out more services as I go.

### I'm mostly using Amplify, Route 53 and S3

I stumbled upon Amplify almost accidentally.

The repo I forked is powered by Jekyll, and one of the big selling points was how easily one could deploy on <a href="https://pages.github.com">GitHub Pages</a>. But I was ride-or-die AWS. So I started searching for a similar kind of plug-and-play deployment option. Lo and behold, AWS Amplify did exactly that.

All I had to do was link up my forked repo's master branch to Amplify, make a few clicks, and the site was live.

### But what about that custom domain?

Here's where Route 53 entered the fold.

A few months ago, I did the yeoman's work of swapping the registration from Hover to Route 53, which is the AWS Domain Name System (DNS) service. The process was a bit of a pain. But it paid off when the time came to deploy the Amplify app. The tight integrations across services meant an extra couple clicks was all it took to have the site up and running at my personal domain.

I'm hoping to figure out how to use S3 image URLs in blog posts like this one. Right now I have to store them locally. But that's the S3 explanation.

### The bottom line

The website is up. I'm pleased. My total AWS bill is about $5/month — a solid savings compared to, say, Squarespace's business plan ($18/month).

And the personal growth? Priceless.