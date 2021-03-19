---
title: "Blog #2 | A non-technical guide on making a clean personal website for professionals (WIP)"
subtitle: A step-by-step guide to set up a professional website and/or blog using Academic theme startkit for Wowchemy, a website builder for the static site generator (SSG) Hugo.

# Summary for listings and search engines
summary: A step-by-step guide to set up a professional website and/or blog using Academic theme startkit for Wowchemy, a website builder for the static site generator (SSG) Hugo.

# Link this post with a project
projects: []

# Date published
date: "2021-03-15T20:28:00Z"

# Date updated
lastmod: "2021-03-15T20:28:00Z"

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
  caption: '[**Codepie**](https://www.flickr.com/photos/135936104@N02/34271173264)'
  focal_point: ""
  placement: 2
  preview_only: true

authors:
- admin

tags:
- Academic
- Wowchemy
- Hugo
- Blog
- Website

categories: []

---

## Initial setup

Daniel Quintana's guide using Wowchemy, Hugo, Github, and Netlify. You will receive 100 GB Bandwidth and 300 Build Minutes per month on a free Netlify Starter Plan, which is more than most will need, regardless of how many times you plan to update the site or blog entries. Registering your own domain name is optional; it is a very cheap subscription, if you use Namecheap, as they suggest, and it will very easily integrate with Netlify.

You have the option to set up full Academic template or just a blog. I would personally encourage everyone to set up the full Academic theme; I believe everyone should have their own space where they introduce themselves. You can look over the various available [templates](https://wowchemy.com/templates/) from Wowchemy to decide. Assuming you follow that advice, my next personal suggestion: follow the newest [2020 guide](https://www.dsquintana.blog/create-an-academic-website-free-easy-2020/) step by step to get the site running as quickly as possible, modifying any steps as desired. Then, visit the "outdated" [2019 guide](https://www.dsquintana.blog/free-website-in-r-easy/) and skim over to the other personalization parts not covered/finished in the newer guide. Modify those instructions as needed to accomodate the newer Wowchemy version and follow those steps, too, as desired. If you do this, it will assist you in doing most of the personalization of your site, step-by-step. Who doesn't like a helping hand?


Documentation that will be helpful - Page Features, Page Elements, and the rest of Docs
Once you have taken the time to go through those guides, you will likely see that there are plenty of other options for personalizing the site to your needs and liking that are not covered. Fortunately, there is extremely thorough and thoughtful documentation provided by the creator.
https://wowchemy.com/docs/content/page-features/
https://wowchemy.com/docs/content/writing-markdown-latex/


## (Optional) The blog

Setting up the blog section of the website, assuming you used the full Academic template from which you remove the Posts widget from the Widget page. Make navigation bar link work, and modify title and entry appearance. Thumbnail images vs. featured image.
If you do not have a Posts widget active on your homepage, remove `#post` and add `/post/` to the `Blog` navigation link `url` setting in `menus.yaml`. This will make sure that the nav. link in the menu will take someone to the archive page, which looks like a traditional blog page you'll find using most platforms. My own website is set up this way.
If you would like to change the title that appears on the archive page of the blog, that can be done by opening (website root)/content/post/_index.md and changing the title to your preference.


## (Optional) To enable comments or not to enable comments

In my opinion, the choice regarding whether or not to enable and allow comments on your site (or which parts of the site you prefer) is a decision that likely rests on how active you wish to remain on other social media platforms. If you are choosing to make this site as a way of starting to divest yourself from the modern digital ghettos we've all electively adopted and given our lives too, then you may wish to have some ability to interact with people who visit your site. However, perhaps you will remain active on other platforms; in that case, trying to manage the comments on the site and the same workload you usually deal with on other platforms may become overwhelming. (Author's note: I used to moderate a Telegram group with tens of thousands of accounts in it that focused on XRP (most of which were bots), and my experience indicates that it is possible for moderating your own site's comments to be more work than you think it will be, depending on how much traffic you drive.)
https://wowchemy.com/docs/guide/comments/
https://wowchemy.com/docs/guide/comments/#choose-where-users-can-comment


## (Optional) Coil Monetization

Site-wide monetization with Coil payment pointer using a customized header.
Coil is an attempt to remove the need for advertising revenue from content produced for the web in order to reward creators by micropayments. The model incorporates a small subscription paid to Coil and installing an extension in your a web browser. Whenever a person visits a web page that is web monetized with appropriate code provided by Coil to creators, the extension installed on that person's browser will stream a small donation to the creator that is paid via the Interledger Protocol. It is incredibly powerful tech that could fundamentally change the way we generate revenue around the web; you can read more about Coil [here] (https://coil.com/).
It took me a while of drilling into the folder hierarchy of my website files, looking for the answer, before I finally gave up and went to the Wowchemy Discord forums. It turns out, I was completely looking at the wrong approach and location to make modifications. I am thankful that there is such a generous community support around this project; in particular, I would like to give a nod to Rodrigo Alcaraz de la Osa, an incredibly talented individual, for his assitance in helping me find the solution to this step. It turns out, modifying the header section of Wowchemy, such that the same modified code shows up on every web page, is very easy. It's also a modification that is discussed in 


## Updating the site
Wowchemy regularly undergoes updates that are detailed in the builder's blog. As suggested by the Update Guide of the Wowchemy Docs, one should look to the relevant blog posts that occur between the time of your latest Wowchemy update and apply the Breaking Changes whenver attempting the next update. It is helpful to regularly check in on the blog and read over the news, because the reasons for making changes are usually detailed, and you'll get information on *why* you would want to update.
https://wowchemy.com/blog/


## (Optional & Advanced) Self-hosting

(for the ambitious who want to own their data and web services).
Assuming that your site will not be driving a tremendous volume of traffic that really demands the highest grade hardware and support available to keep up with demand, you may want to give self-hosting a try. This is the ultimate step in ensuring that your content is as censorless as possible on the open web. Will Ho wrote a great blog post detailing how to set this up and what considerations are needed.
https://ikarus.sg/how-i-started-self-hosting/?ref=hackernoon.com


Over time, I have accumulated a number of topics that, when I encounter them, I will say something like, "Yeah, that's really important; I should work on that," or the like. Learning the how and why of working with computer code, registering for and using a Git version control system like GitHub, learning why plain text files can be very helpful and useful, and setting up a personal website and blog are topics that fall on that list. However, it seems like life always gets in the way, somehow, and I never get around to it. Then, this past year and a half happened and, with it, a number of events (such as remote work and the simultaneous deplatforming of people from social media for reasons that could be used against anyone at any time) that cast a 1 million watt flashlight on the face of this sleeping man, and I couldn't avoid the matters any lnoger. Not only had I always wanted to work on these things, but the world also seemed to be presenting me with the exact circumstances that led me to think they were good ideas in the first place. So, I set out to work on these things.

When I was in the midst of setting my blog up, I knew that one of the first entries I should make was to highlight the process I used. It turns out that there are tools and guides out there that make setting up a clean and professional personal website and/or blog incredibly easy. If you are not familiar, the process that this blog highlights to accomplish this is referred to as a Static Site Generator (SSG). Basically, You don't have to know how to code a website yourself. The generator (such as Hugo, Gatsby, or Jekyll) does the hard part for you, and most of the customization required of the use is modifying plain english files that use simple markup language. The generator reads those markup language files you create and uses repositories of advanced scripts and coding languages to actually make the site for you. Furthermore, most templates available, usually completely free of charge, come pre-made with all of the files needed to ensure the site is whole; simply follow the documentation the template maker provides and modify the markup language files as needed. If you ever wish to modify the website, that is quite easy; you modify the same files and reupload them for building and deployment. It's all very smooth and seamless; anyone who has ever tried to write a website from scratch can attest that putting together a professional personal website from scratch can be difficult for beginners. SSGs are truly a chance for people to set up a clean website, with as little fuss as possible, that belongs to them - a place for them to explore and express themselves.

When I made the committment to this endeavor, I began searching for a good solution to setting up a professional website, one which came with a guide that could help me get up and going quickly and provide me with quick, observable positive reinforcement that showed me I was doing things correctly. I came across and blog entry from Daniel Quintana and, when I read it, saw how easy it was, and looked at the results, I knew I found my solution. I also have read a plehora of people in the development communities who are switching away from typical blogging platforms like Wordpress and Ghost and go with a SSG and chose Hugo. The reviews I've read have been very positive of it, and I feel similarly. 


## References:

Cushen, G. (2021, March 15). Wowchemy Docs [Static]. Wowchemy: Free Website Builder for Hugo. https://wowchemy.com/docs/

Quintana, D. S. (2020, September 29). Create an academic website for free in under an hour [Blog]. Dsquintana.Blog. https://www.dsquintana.blog/create-an-academic-website-free-easy-2020/

Quintana, D. S. (2019, June 15). How to make a free personal website in R [Blog]. Dsquintana.Blog. https://www.dsquintana.blog/free-website-in-r-easy/

