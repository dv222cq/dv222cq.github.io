---
layout: post
title:  "On Static Site Generators (SSGs)"
date:   2019-11-12 00:17:59 -0600
categories: ssg
image: /assets/og-david.jpg
---
This site is implemented through [Jekyll](https://jekyllrb.com/){:target="_blank"}, an SSG, or Static Site Generator. SSGs are frameworks for simplifying development and maintenance of _static_ web sites, trough techniques like _includes_, _variables_, _layouts_, etc. I.e. "_Don't Repeat Yourself_".

Arguing for SSGs' usefullness, [Eduardo Bouças (2015)](https://davidwalsh.name/introduction-static-site-generators){:target="_blank"} gives an analogy of a news kiosk where the newspaper has to be created by a team of professionals upon each customers request. It's a big waste of resources. So can platforms for dynamically generated web sites (e.g. [Wordpress](https://wordpress.com/){:target="_blank"}) be in many cases. Bouças presents SSGs as a process where the newspaper is recreated only when news happen. Not every time a customer requests a copy.

**So SSGs are frameworks generating flat, basic web sites from an archive of content files, upon _change_ of the content – not upon every retrieval request.** The approach makes sense, as illustrated by Bouças' analogy. There are limitations, as explained by Bouças and others, but it's a matter of prioritization of features and choosing the appropriate tool for the task at hand.

As indicated in [my bio](/about/), I've been around the web development business for a while, seeing and trying some stuff using different methods and platforms. My issue with frameworks and platforms has always been the **return on investment**. You've got to _research the pros and cons_ of each framework and usually choose from competitors. Then the framework must be _learnt_. Learning means getting to grips with the basic interface and documentation, and usually researching specific hacks for each specific projects. This often involves learning about the framework's dependencies again. **In sum, I've never found this task trivial at all. And throughout the years, frameworks and abstractions have come and gone.**

My experience with Jekyll has reflected this pattern: I've had to learn the framework through it's basic interface and documentation, then proceed to find solutions and hacks for specific requirements – even for a site as simple as this. There's a significant overhead.

For a professional developer needing to build quick & simple pages every now and then, this overhead seems a lesser ask. But a friend of mine who's been professionally developing small to medium sized web sites for decades, replied that he'd rather just go ahead with the usual Wordpress-installation anyways.

**I wonder if SSGs might not fall between chairs – being appropriate for too small a niche to justify the overhead of learning (and keeping up with) the frameworks?**

Even small sites often require some dynamic content, and customers have genuine needs for the UI offered by content management systems that should be taken seriously. Suggesting users use new terminology and syntax for basic content also seems like an ill-advised idea to me. Why would I want to learn to implement images with: `[![alt text][image]][hyperlink]` rather than good old: `<a href="hyperlink"><img src="image" alt="alt text"></a>`? It's just learning new syntax that's only applicable on this particular framework. Not really easier either. And what do I do when I want links to open in a new tab? _Heading back to Google/Stack Overflow again…_

[Google Trends](https://trends.google.com){:target="_blank"} show increasing interest for SSGs from 2013 and onwards, seemingly flattening out a bit, but not decreasing:

<figure>
<a href="https://trends.google.com/trends/explore?date=all&q=static%20site%20generator" target="_blank"><img src="/assets/trends-ssg.png" alt="Line diagram showing increasing interest for Static Site Generators on Google Trends" /></a>
<figcaption>Line diagram showing increasing interest for Static Site Generators on Google Trends</figcaption>
</figure>

**Personally, I'm primarily intrigued by the idea of generating simple, flat web content, ready to be served in any amount, at any time. Includes, templates and layouts are more clever than using PHP-includes and templates, as I've been used to.**

It seems highly relevant for quick & easy creation of sites for personal projects and portfolios. But I can't envision delivering a Jekyll-based project to a customer, telling them they have no access to editing the content, nor explaining them how to do it "the Jekyll way". Not at this point in time.
