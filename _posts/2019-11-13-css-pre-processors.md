---
layout: post
title:  "Using CSS Preprocessors"
date:   2019-11-13 00:17:59 -0600
categories: css-preprocessors
image: /assets/og-david.jpg
---
I was very comfortable with HTML and CSS back in the days, and had a significant interest in "working smart – not hard". I read up on different resources, like the [Wordpress style guide](https://make.wordpress.org/core/handbook/best-practices/coding-standards/css/){:target="_blank"}, [Object Oriented CSS](https://www.smashingmagazine.com/2011/12/an-introduction-to-object-oriented-css-oocss/){:target="_blank"} (OOCSS) and [Inuit CSS](https://github.com/inuitcss){:target="_blank"}.

Here's how they're trending these days:

<figure>
<a href="https://trends.google.com/trends/explore?date=all&q=%2Fm%2F01028j2g,inuit%20css" target="_blank"><img src="/assets/trends-oocss.png" alt="Line diagram showing dying interest for Object Oriented CSS" /></a>
<figcaption>Line diagram showing dying interest for Object Oriented CSS</figcaption>
</figure>

Then came SASS, LESS and other CSS preprocessors, making things even more interesting. Alas, I didn't have the technical proficiency for setting up the environment, nor the time to prioritize and learn. During this course, I got the chance to revisit it though.

Now, CSS preprocessors, are frameworks generating plain vanilla CSS from input utilizing the framework's own syntax and functionality. The point is keeping development <abbr title="Don't Repeat Yourself">DRY</abbr>. Reading up on streamlining stylesheets, I'd learned that it's quite common for stylesheets to have literally _hundreds_ of references to the same color, the same font stack etc. With preprocessors, style guides could be implemented and maintained through variables, which to me seemed like a stroke of genius. Other common features are nested rules, inheritance and mixins.

We were warned by the course instructor that this might be the last time he'd teach CSS preprocessors due to declining general interest as a result of developments within CSS freeing developers from the need. Looking it up on Google Trends (again) seemed to indicate decent interest anyways:

<figure>
<a href="https://trends.google.com/trends/explore?date=all&q=scss" target="_blank"><img src="/assets/trends-scss.png" alt="Line diagram showing increasing – perhaps at its high water mark – interest for Sassy CSS, specifically." /></a>
<figcaption>Line diagram showing increasing – perhaps at its high water mark – interest for Sassy CSS, specifically.</figcaption>
</figure>

Compared to regular CSS, preprocessors allow **DRYer and more structured stylesheets, which should be easier to maintain**. It's unfortunate that preprocessors' structuring and nesting cause unnecessary specificity and "bloat", i.e. "ugly" output CSS.

Considering this use case, using Jekyll, I've already stated that I see Static Site Generators as most appropriate for private projects of a lesser scale. CSS preprocessors on the other hand, show their advantages on the grander scaled projects, so I see a inconsistency here. There shouldn't be a need for preprocessing the CSS of quick & easy static web sites.

As for my use of SASS in this project, I've tried to implement the different features despite keeping things simple, i.e. not changing a lot from the default "minima" theme.

details…
