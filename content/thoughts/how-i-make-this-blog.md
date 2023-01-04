+++
title = "How I Made This Blog"
author = ["Christian Elliott"]
date = 2022-11-26T00:00:00-06:00
lastmod = 2022-11-26T00:00:00-06:00
draft = false
+++

A summary of how this blog is constructed and my blogging workflow


## It All Starts With Org Mode {#it-all-starts-with-org-mode}

Emacs' [Org Mode](https://orgmode.org/) has been a really critical discovery in the last couple years of
my life. At some point or another, I decided I wanted to truly revamp my
personal organization, in essentially all regards. I have always struggled with
note taking and keeping a planner and even maintaining any kind of TODO lists.
In short, my personal organization didn't exist before Org Mode. Nevertheless,
it does now.

I won't go too far into explaining Org Mode, since the motivated reader can
Google themselves. But in summary, it is a Markdown-esque system that works on
plain text files. The "mode" part (where the magic really happens) lives in
Emacs. It is safe to say that the benefit of Org Mode can only be fully
understood if using it within Emacs, and that is perhaps seen as a blessing to
some and a curse to others. Personally, I love Emacs. But I am already
encroaching on dangerous ranty territory if I continue in this direction, so I
shall move along.

To be certain, mentioning Emacs' org-mode is necessary because it is the basis
for my whole workflow. I write in Org Mode. I note take. I journal. I plan. I
sometimes code. I create in Org Mode. So when I set out to make a blog, it
needed to encorporate my Org Mode workflow.


## Design Decisions {#design-decisions}

The next step in determining how to create my blog was a more challenging
and impactful choice. As stated, the actual content of my blog needed to come
from an org file, but otherwise there were really no limiting parameters. I
weighed the option of generic web application, e.g. React on Rails (since I am
familiar with that from work), but frankly even that seemed overkill for my
"blog" want. I just wanted to take my content and have it sent straight to my
blog. Simple... right?

At work I've also utilized some Github Pages documentation sites. Github Pages
itself defaults to using Jekyll, a [static site generator](https://en.wikipedia.org/wiki/Static_site_generator). So I already had some
knowledge of static site generators and what they are used for. It didn't take
much Googling to discover that Emacs already has tools like [weblorg](https://emacs.love/weblorg/) and [others](https://orgmode.org/worg/org-blog-wiki.html)
to assist in the content-to-blog workflow I was seeking. It became obvious quite
quickly that utilizing a static site generator would be my best bet, since I
didn't seek any other functionality and they are fairly simple in general. With
this setup, there'd be no manually setting up routes or configuring certain
controllers as I would in a RoR app - not to mention that I could grab a free
theme and get started almost immediately on deploying the site.

In the end, I liked the way [ox-hugo](https://ox-hugo.scripter.co/) approached the workflow I was looking for.
It prioritizes the option for keeping all your content in a single org file
(called subtree exporting), which simplifies things a lot for me. I can view all
of my blog's content in one place, and manage the export location in the
subtree's metadata. If you're familiar with web development, the name ox-hugo
might have also clued you in on my static site generator of choice: Hugo. In
making this decision about ox-hugo I essentially killed two birds with one
stone, and didn't have to spend anymore time looking at the pros and cons of,
say, Jekyll, Hugo, etc. All that remained was to choose my theme.


## It's Gotta Look Good {#it-s-gotta-look-good}

To me, the look and feel of any application or website is everything. Frankly, I
am a very novice software engineer and have no experience with UI/UX design, but
I do know a good color scheme when I see one (tangential self-plug: I'm writing
this in [Doom Emacs using the Zenburn palette](/img/how-i-make-this-blog/doom-emacs-zenburn.png) - it's pure joy). It took about a
day for me to stumble upon the simple [Blowfish](https://github.com/nunocoracao/blowfish) theme and I really enjoy it. I
wanted something that was both minimal and pleasant to look at. I think Blowfish
accomplishes this nicely, and it comes with a lot of features to boot. Honestly
I'm a little surprised by the fact that it has a relatively small number of
Github stars. After about three weeks of getting familiar with it, I don't have
any major complaints.


## End {#end}

I debated for a while about how technical I'd get with this post. However, being
detailed and retracing my steps for setup and initial deployment and the Github
Pages stuff would take a decent amount of extra time, and right now I am
prioritizing producing content for my blog, not on making tutorials. So that's
where I will end things! I am _really_ enjoying the setup I'm using. That part
is important to me, because if I don't enjoy it, I'll stop doing it.

If you've made it this far, thanks and cheers.
