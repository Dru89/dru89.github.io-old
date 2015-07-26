---
layout: post
date: 2013-03-16 15:48:00
comments: yes
slug: moving-on-from-posterous
summary: 'Posterous is gone.  Long live Jekyll.'
title: 'Moving on from Posterous'
tags:
- jekyll
- blogs
- posterous

---

This is my first post using [Jekyll](http://jekyllrb.com/) as my blogging engine. With [posterous shutting down](http://blog.posterous.com/thanks-from-posterous), I felt like I had to find a new alternative.  I don't blog often, but I wanted a system that I felt like would last, in case the next site I chose shut down, too.  That means that my system should be self-hosted, if necessary.

Also, I love writing in [Markdown](http://daringfireball.net/projects/markdown/syntax).  I write my notes in it, and it stands to reason that my blogs would be well written in the sytnax as well.

With this knowledge, I decided to look into several different options.  The first option was [Wordpress](http://wordpress.org/).  I created an [EC2](http://aws.amazon.com/ec2) micro instance and installed Wordpress on it.  It was a rather simple process, and I found some useful plugins.  Unfortunately, none of them quite fit the way that I wanted them to.  They all required me to use some external editor to really get my code formatted correctly, but still required the use of a database.  And worst of all, they didn't use [Github Flavored Markdown](https://help.github.com/articles/github-flavored-markdown).

Enter [Jekyll](http://jekyllrb.com/).  I can use whatever hosting I want, ec2 instances, my own host, or even [Github Pages](http://pages.github.com/).  Jekyll takes my content and generates static pages for it.  I can use my own layout, as well.  It's all based on [liquid](http://liquidmarkup.org/), which reminds me a lot of [Django templates](https://docs.djangoproject.com/en/dev/topics/templates/), so it's pretty easy to write.  When I'm ready to publish my blog posts, I can just push them and they're ready to go.

I'm not going to say it's perfect, but it is pretty good.  I think it will work out well for my once-in-a-while blogs.

**Edit:** I'm aware that tags aren't working right now.  I think that's a side-effect of using Github Pages for this.  They don't seem to allow extra plugins.  I'll see if I can find a work-around later.

Also, if you're interested in seeing the source code for the blog, you can find it here: <https://github.com/Dru89/dru89.github.com>

**Edit 2:** I've fixed the tags problem by moving to an ec2 micro-instance.  One of the upsides of being so portable I guess is easily moving things around.

I added a git hook that automatically rebuilds the static site whenever I push changes to it.  This should be fun.

**Edit 3:** Final edit, I swear.  I just found out how to import all of my old posts to Jekyll: <https://github.com/mojombo/jekyll/wiki/Blog-Migrations>