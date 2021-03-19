---
title: "Blog #2 | A non-technical guide on making a clean personal website for professionals"
subtitle: A step-by-step guide to set up a professional website and/or blog using Academic theme startkit for Wowchemy, a website builder for the static site generator (SSG) Hugo.

# Summary for listings and search engines
summary: A step-by-step guide to set up a professional website and/or blog using Academic theme startkit for Wowchemy, a website builder for the static site generator (SSG) Hugo.

# Link this post with a project
projects: []

# Date published
date: "2021-03-19T20:28:00Z"

# Date updated
lastmod: "2021-03-19T20:28:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# To use, place an image named `featured.jpg/png` in your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
# Set `preview_only` to `true` to just use the image for thumbnails.
image:
  caption: '[**racheocity**](https://www.flickr.com/photos/34247648@N02/4298911131)'
  focal_point: ""
  placement: 2
  preview_only: true

authors:
- admin

tags:
- Academic
- Wowchemy
- Hugo
- Coil
- Interledger Protocol
- Blockchain
- Blog
- Website

categories: []

---

Over time, I have accumulated a number of topics that, when I encounter them, I will say something like, "Yeah, that's really important; I should work on that," or the like. Learning the how and why of working with computer code, registering for and using a Git version control system like GitHub, learning why living in plain text files can be very helpful and useful, and setting up a personal website and blog are topics that fell on that list. Previously, it seemed like life always got in the way, and I never get around to it. Then, this past year and a half happened, and, with it, a number of events (such as remote work and the simultaneous deplatforming of people from social media for reasons that could be used against anyone at any time) took place that cast a 1 million lumen light on the face of this sleeping man, and I couldn't avoid the matter any longer. Not only had I always wanted to work on these things, but the world also seemed to be presenting me with the exact circumstances that led me to think they were good ideas in the first place. When I was in the midst of setting up the Blog, I knew that one of the first entries I should make was to highlight the process I used to create my website and blog; here we are. It turns out that writing this entry was easier than I thought it would be, because the process was made so simple using the tools and resources I chose.

## Initial setup

When I made the committment to this endeavor, I began searching for a good solution to setting up a professional website, one which came with a guide that could help me get up and going quickly and provide me with quick, observable positive reinforcement that showed me I was doing things correctly. I came across a blog entry from [Dr. Daniel Quintana](https://www.dsquintana.com/) and, when I read it, saw how easy it was, and looked at the results, I knew I found my solution. I also have read thoughts from a plehora of people in the development communities who are switching away from typical blogging platforms like Wordpress and Ghost to go with a SSG (such as Hugo, Gatsby, or Jekyll) and chose Hugo to do so. The reviews I've read have been very positive of it, and my experience with Hugo echos those reviews.

Dr. Quintana writes an annual [guide](https://www.dsquintana.blog/create-an-academic-website-free-easy-2020/) for beginners on using Wowchemy and Hugo to create a clean personal website in a matter of minutes that is completely free. Your website files created by Wowchemy will be hosted on GitHub; Netlify will build and deploy the website from the GitHub hosted files. [Registering your own domain name](https://wowchemy.com/docs/guide/domain/) is completely optional but highly encouraged. Registering the domain is a very cheap yearly subscription (usually a few USD for a .com), if you use Namecheap (as Wowchemy suggests); also, I can attest that integrating the custom domain from Namecheap with Netlify was a cinch.

With Wowchemy, you have the option to set up full Resume template or just a Blog. I would personally encourage everyone to set up the full Resume theme; I believe everyone should have a space they control, where they introduce themselves and their work product to people (like an electronic business card and portfolio combined). You can look over the available [templates](https://wowchemy.com/templates/) from Wowchemy to decide on your preference. Assuming you follow my advice, my next personal suggestion: follow his newest [2020 guide](https://www.dsquintana.blog/create-an-academic-website-free-easy-2020/) step by step to get the site running as quickly as possible, modifying any steps as desired. Next, decide if you want to [register the optional domain name](https://wowchemy.com/docs/guide/domain/) (and do it or don't). Then, visit his "outdated" [2019 guide](https://www.dsquintana.blog/free-website-in-r-easy/) and skim over to the other personalization parts not covered/finished in the newer guide. Modify those instructions as needed to accomodate the newer Wowchemy version and follow those steps, too, as desired. If you do this, it will assist you in doing most of the personalization of your site, step-by-step. Who doesn't like a helping hand?

Once you have taken the time to go through those guides and you possess an operational site to your liking, you will likely see that there are plenty of other options for personalizing the site to your needs and liking that are not covered in the guides. Fortunately, there is extremely thorough and thoughtful [documentation](https://wowchemy.com/docs/) provided by the creator. In particular, I suggest you review the ["Getting Started,"](https://wowchemy.com/docs/getting-started/get-started/) the ["Page Features,"](https://wowchemy.com/docs/content/page-features/) and the ["Page Elements"](https://wowchemy.com/docs/content/writing-markdown-latex/) sections; the entire Docs compilation is important to go through in time, though.

One customization I made is that I changed the title of the `Posts` page to `Blog` in the appropriate file located at `(website root)/content/post/_index.md` and made the necessary update to the title of the blog section in the navigation menu, too, by updating the file located at `(website root)/config/_defualt/menus.yaml`. I also changed the style of `View` for the posts page to `Card`.

There are some quick key customizations I think you should consider implementing that are detailed next, so read on.

## (Optional) I do not have a blog widget on the homepage; how do I link to the archive of my blog posts?

{{% callout note %}}
This section is for those who wish to have a link to their blog posts archive in the navigation menu and who set up the full Resume template **and** did not set up a posts widget on the the home page. 
{{% /callout %}}

If you do not have a Posts widget active on your homepage, remove `#post` and add `/post/` to the `Blog` navigation link `url` setting in `menus.yaml`. This will make sure that the navigation menu link will take someone to the archive page, which looks like a traditional blog page you'll find using most platforms. My own website is set up this way.

If you would like to change the title that appears on the archive page of the blog, that can be done by opening `(website root)/content/post/_index.md` and changing the title to your preference.

## (Optional) To enable comments or not to enable comments

{{% callout note %}}
If you have zero interest in enabling a commenting system on your website, you can skip this section.
{{% /callout %}}

In my opinion, the choice regarding whether or not [to enable and allow comments](https://wowchemy.com/docs/guide/comments/) on your site (or [which parts of the site you prefer to allow comments](https://wowchemy.com/docs/guide/comments/#choose-where-users-can-comment)) is a decision that likely rests on how active you wish to remain on other social media platforms. If you are choosing to make this site as a way of starting to divest yourself from the modern digital ghettos we've all electively adopted and given our lives too, then you may wish to have some ability to interact with people who visit your site. However, perhaps you will remain active on other platforms; in that case, trying to manage the comments on the site and the same workload you usually deal with on other platforms may become overwhelming. (Author's note: I used to moderate a Telegram group with tens of thousands of accounts in it that focused on XRP (most of which were bots), and my experience indicates that it is possible for moderating comments to be more work than you think it will be, depending on how much traffic you drive.)

## (Optional) Coil Monetization

{{% callout note %}}
If Coil web monetization of your website is not something you wish to do, you can skip this section.
{{% /callout %}}

Coil is an attempt to remove the need for advertising revenue from content produced for the web in order to reward creators by micropayments instead. Website viewers who want to support this model can pay a small monthly subscription to Coil and install an extension in their a web browser. Whenever a person visits a web page that is web monetized, the extension installed on that person's browser will ensure that a small revenue is paid to the creator via the Interledger Protocol, a blockchain web protocol. It is incredibly powerful tech that could fundamentally change the way we generate revenue around the web; you can read more about Coil [here] (https://coil.com/) and [here](https://help.coil.com/docs/monetize/intro-to-monetization) and Interledger Protocol [here](https://interledger.org/).

In order to monetize content on your site, you will need to [sign up for a free Creator account](https://coil.com/signup?type=creator); if you already have a Coil Creator account, you can skip this step. Log into your account and look to the top right (next to "+ New Post") and click on that menu and select ["Settings."](https://coil.com/settings/account) The tab you are looking for is ["Monetize Content."](https://coil.com/settings/monetize) However, if you haven't done so, yet, you will need to set up a blockchain wallet provider for payouts via the ["Payouts" tab](https://coil.com/settings/payouts). Choose whichever blockchain service you wish to use and, if necessary, set up an account with them.

It took me a while of drilling into the folder hierarchy of my website files, looking for the answer, before I finally gave up and went to the Wowchemy [Discord Server](https://discord.gg/z8wNYzb) forums. It turns out, I was completely looking at the wrong approach and location to make modifications. I am thankful that there is such a generous community support around this project; in particular, I would like to give a nod to [Rodrigo Alcaraz de la Osa](https://twitter.com/alcarazr), an [incredibly talented individual](https://fisiquimicamente.com/), for his assitance in helping me find the solution to this step. It turns out, modifying the header section of Wowchemy, such that the same modified code shows up on every web page header, is very easy. It also turns out that the instructions are included in the official Wowchemy Docs (albeit in a slightly hidden place).

In order to monetize your content, you will need to place a file called `custom_head.html` in `(website root)/layouts/partials`, as described [here](https://wowchemy.com/docs/guide/extending-wowchemy/#custom-head). In the `custom_head.html` file you create, place the code provided to you by Coil in your ["Payouts" tab](https://coil.com/settings/payouts). The code will look something like the following:  `<meta name="monetization" content="(your ILP Payment Pointer)">`, where the `content` portion will contain an [ILP Payment Pointer](https://help.coil.com/docs/monetize/paymentpointer/pp-overview/index.html) that references whichever service you created an account with to set up the appropriate wallet.

Once you have updated your website files and pushed the updates to GitHub for deployment, you can check to make sure your setup is working correctly by installing the [Coil browser extension](https://help.coil.com/docs/membership/coil-extension) and visiting your site. If the setup was done correctly, when you click on the Coil extension, it will tell you that the website is monetized. Congratulations - you now have an ability to earn revenue from the content you produce!

## Updating the site

Wowchemy regularly undergoes updates that are detailed in the builder's blog. As suggested by the Update Guide of the Wowchemy Docs, one should look to the relevant blog posts that occur between the time of your latest Wowchemy update and apply the Breaking Changes whenver attempting the next update. It is helpful to regularly check in on the blog and read over the news, because the reasons for making changes are usually detailed, and you'll get information on *why* you would want to update.
https://wowchemy.com/blog/.

I also used my [first blog post](https://www.dbbrunson.com/post/entry00001/) to keep the important information and links that are present in the Example Blog Post that comes with the initial setup of the Academic Theme from Wowchemy. There may be information of interest for you there as well.

As of this point, you can consider this guide finished. The final section of this post is only meant for advanced users who have some experience with maintaining servers. The chances are, if this guide is of any actual use to you, the next section is not adviseable for you to attempt.

## (Optional & Advanced) Self-hosting

{{% callout warning %}}
This section is only for the ambitious, who want to own their data and web services; however, it is not for the Faint of Heart.

If you attempt this section and have issues with making it work correctly, I will not be a good person to contact for help.

You are hereby warned.
{{% /callout %}}

Assuming that your site will not be driving a tremendous volume of traffic that really demands the highest grade hardware and support available to keep up with demand, you may want to give self-hosting a try. Self-hosting is the act of maintaining the hardware needed to serve a service, such as a website, to people who are using the appropriate address information to find it. In the context of this blog post, self-hosting would replace the need for GitHub and, depending on your choices, Namecheap. This is the ultimate step in ensuring that your content is as censorless as possible on the open web. Will Ho wrote great blog posts [here]](https://ikarus.sg/how-i-started-self-hosting/?ref=hackernoon.com) and [here](https://ikarus.sg/how-i-built-kraken/) detailing how to set this up and what considerations are needed. I will leave it to his better abilities to explain how to go about accomplishing this. Best of luck to you on this endeavor!

## References:

Cushen, G. (2021, March 15). Wowchemy Docs [Static]. Wowchemy: Free Website Builder for Hugo. https://wowchemy.com/docs/

Quintana, D. S. (2020, September 29). Create an academic website for free in under an hour [Blog]. Dsquintana.Blog. https://www.dsquintana.blog/create-an-academic-website-free-easy-2020/

Quintana, D. S. (2019, June 15). How to make a free personal website in R [Blog]. Dsquintana.Blog. https://www.dsquintana.blog/free-website-in-r-easy/

