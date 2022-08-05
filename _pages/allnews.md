---
title: "Corail Research Group - News"
layout: textlay
excerpt: "Corail Research Group - News"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em>
{% if article.image != nil %}
<img src="{{ site.url }}{{ site.baseurl }}/images/miscpic/{{ article.image }}" class="img-responsive" width="100%" style="float: left" />
{% endif %}
</p>
{% endfor %}
