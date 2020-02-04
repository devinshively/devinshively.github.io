---
layout: post
title:  "New To Jekyll"
date:   2020-01-31 18:41:28 -0700
categories: setup
---
Getting started with Jekyll as been interesting.

I have decided to continue to use the provided theme `minima`.

The plugins that I have added are
  - jekyll-seo-tag
  - jekyll-analytics

### Seo Tag
To add the seo tag plugin I first had to create a new folder `_includes`.
Then I had to find my theme's head template. This was found using `bundle info minima`.
Next I copied my theme's `_includes/head.html` to my new folder `_includes`.
Then I added `{% raw %}{% seo %}{% endraw %}` before `</head>` in the newly copied file.

### Analytics
I added the below to `_config.yml` to get google analytics working:
{% highlight yml %}
jekyll_analytics:
  GoogleAnalytics:          # Add, if you want to track with Google Analytics
    id: UA-????????-?       # Required - replace with your tracking id
    anonymizeIp: false      # Optional - Default: false - set to true for anonymized tracking
{% endhighlight %}

### Fav Icon
To added the image I wanted to use as the fav icon to my project as `favicon.png`.
Then I edited `_includes/head.html` adding `{% raw %}<link rel="shortcut icon" type="image/png" href="favicon.png">{% endraw %}` right before `{% raw %}<link rel="stylesheet" href="{{ "/assets/main.css" | relative_url }}">{% endraw %}`.


### Embedding images:
![This is an image of a squirrel](/images/squirrel.jpg)

I am constantly having to go back and reference the [Jekyll docs][jekyll-docs].

[jekyll-docs]: https://jekyllrb.com/docs/home

