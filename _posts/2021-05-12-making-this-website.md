# making this website

I needed a website. So I finally got my shit together and made one.

For a long time, I used Squarespace templates for my personal website. It got the job done alright. Squarespace sites can be really slow. They're customizable, sort of. But it wasn't enough.

I then got to thinking, "Why should I spend my hard-earned dough on some mass-produced template built by a private enterprise, when I could just make one myself and have total control over it?"

Control is the key. [Own the master](https://www.amuse.io/content/owning-your-masters?cn-reloaded=1). Whenever possible in life, you have to own the master.

### the tools

I found this template on GitHub and forked the repo. It's called al-folio.

It's working pretty well so far. I wanted something with a blog functionality and I like how this one lets me write entries in Markdown and make simple customizations to metadata. Something like Wordpress felt like overkill given that I probably won't be posting here too often. Markdown is clean, simple and lightweight. (Plug: I wrote this post in a great macOS app called MacDown.)

All the code is stored in a GitHub repo. From there, everything else is AWS.

I used to host this domain (which my dad nabbed many moons ago — thanks dad!) on Hover. But I knew I wanted to run and manage everything from AWS. I wanted to teach myself how it all worked given that it's basically the industry standard. AWS is also highly integrated and well-documented.

Sure, the scale at which I'm using AWS is microscopic. But I've learned a lot about it throughout this process and I'm interested in examining more services as I go.

The three main services I'm using are Amplify, Route 53 and S3.

I stumbled upon Amplify almost accidentally. The GitHub repo I forked is powered by Jekyll, and one of the big selling points of the repo was how easily one could deploy the site on GitHub Pages. However, because I was ride-or-die AWS, I started searching for a similar kind of plug-and-play deployment through AWS. Lo and behold, Amplify did exactly that. All I had to do was link up my forked repo's master branch to Amplify, make a few clicks, and the site was live.

But what about that slick custom domain?

That's where Route 53 entered the fold. A few months ago, I swapped the registration from Hover to Route 53, the AWS Domain Name System (DNS) service. The process was a bit of a pain , but it paid off when it came time to deploy the Amplify app. The tight integrations across services meant it was an extra couple clicks to have the site up and running at my personal domain.

I'm hoping to figure out how to use S3 image urls in blog posts like this one. Right now I have to store them locally. But that's the S3 explanation.

### the bottom line

The website is up. I'm pleased. Compared to, say, Squarespace's business plan (18/month), my total AWS bill is about 5/month. And the personal growth? Priceless.