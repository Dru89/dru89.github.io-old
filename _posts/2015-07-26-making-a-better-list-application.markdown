---
layout: post
title: "Making a Better List Application"
date: "2015-07-26"
categories: [programming]
tags: [gtd, app]
---

For years, I've had a dream.  Not of peace, ending world hunger, or the perfect sandwich.  No, my dream is much more
mundane.  I dream of the perfect list application.  Why bother, you ask?  List applications are a dime a dozen.  To name
a few:

1. [Wunderlist](https://www.wunderlist.com/)
2. [Any.do](https://www.any.do/)
3. [Todoist](https://en.todoist.com/)
4. [Todo.txt](http://todotxt.com/)
5. ...and [many](https://goo.gl/LK41sx) [more](https://goo.gl/NFxzO3)

But these are not the lists that I want.  I don't want a grocery list that simply looks like:
<ul class="list-unstyled">
  <li class="checkbox"><label><input type="checkbox"> milk</label></li>
  <li class="checkbox"><label><input type="checkbox"> eggs</label></li>
  <li class="checkbox"><label><input type="checkbox"> bread</label></li>
</ul>

What if I want to add a grouping by store that I shop at?  Or possibly sort by the price of the items that I'm buying.
Maybe I prefer a specific brand?  Maybe I want to store metadata like the UPC of the item that I'm buying, or a link to
the item on the store's website.  What if the list is actually landmarks I want to visit, grouped by city?  Or sorted
by distance from my current location?

I have few options at this point.  I can maintain each separate list as an HTML table or Excel spreadsheet, 
painstakingly adding things like geographic location and the ability to group/sort in.  I can keep each list schema as
its own table in a database.

For fun, I'm going to start an open source project called [2do](https://github.com/Dru89/2do).  It should do exactly
this.  I'm not sure how I'll be building it yet, but I'll post more on it as I start developing it.  In truth, this
is not the first time I've tried to do a project like this, but here's hoping that I'll be a little more likely to
follow through this time.

For a quick introduction, I'm looking to build this site with Django as the backend, with a focus on using React as the
frontend.  It should be an interesting experience and a great learning opportunity, at the very least.
