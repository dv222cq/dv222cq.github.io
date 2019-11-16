---
layout: post
title:  "Open Graph in Jekyll"
date:   2019-11-14 00:17:59 -0600
categories: open-graph
image: /assets/og-slack.png
---
"The Open Graph protocol enables any web page to become a rich object in a social graph." ([Open Graph, 2019](https://ogp.me/){:target="_blank"}) In practice, this means Facebook, Slack, Twitter and other platforms may fetch images and descriptions, displaying your link as a "card", rather than a plain text link. Which again translates to user friendliness and considerably more clicks.

<figure>
<img src="/assets/og-slack.png" alt="Screen shot of sharing a link to this site in Slack." />
<figcaption>Screen shot of sharing a link to this site in Slack.</figcaption>
</figure>

Open Graph is implemented simply through adding meta tags in the page `head` section. The following were the Open Graph metadata at the time of writing:

{% highlight html %}
<meta property="og:title" content="Open Graph in Jekyll">
<meta property="og:locale" content="en_US">
<meta property="og:description" content="“The Open Graph protocol enables any web page to become a rich object in a social graph.” (Open Graph, 2019) In practice, this means Facebook, Slack, Twitter and other platforms may fetch images and descriptions, displaying your link as a “card”, rather than a plain text link. Which again translates to user friendliness and considerably more clicks.">
<meta property="og:url" content="https://dv222cq.github.io/open-graph/2019/11/14/open-graph.html">
<meta property="og:site_name" content="David’s space">
<meta property="og:image" content="https://dv222cq.github.io/assets/og-david.jpg">
<meta property="og:type" content="article">
{% endhighlight %}

The default installation of Jekyll with the "minima" theme included features Open Graph metadata, but finding how to use them wasn't so straight-forward. In the end (googling having failed me) I managed to dig out an explanation in the `advanced-usage.md` file, deep down in the vendor-folder. At first specifying the `og:image` on a _per page_ basis, and then also how to define a default in `_config.yml`. This setup provides a default, and permits overriding it when appropriate.

I'm a bit surprised though, that Open Graph should be so readily implemented in the boilerplate, but still so hard to configure. I probably did something wrong. 😅

By the way, I found I had to define `url` (base hostname) in `_config.yml` for the live site for the image to load. Relative paths wouldn't work.

There was also an issue of researching OG image dimensions. Providing an image with 1.9 : 1 dimensions turned out well in the end. My original image caused issues of poor clipping on some platforms.
