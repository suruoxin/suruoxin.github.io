---
title: "Footprints"
layout: gridlay
sitemap: false
permalink: /footprints/
---

## Footprints👣

<div class="footprints-map-wrap">
<div id="footprints-map" data-world="{{ site.url }}{{ site.baseurl }}/assets/data/countries-110m.json" data-footprints="{{ site.url }}{{ site.baseurl }}/assets/data/footprints.json"></div>
<div class="footprints-legend">
<span class="legend-item"><span class="legend-swatch visited"></span>Visited</span>
<span class="legend-item"><span class="legend-swatch"></span>Not visited</span>
</div>
</div>

<script src="https://cdn.jsdelivr.net/npm/d3@7"></script>
<script src="https://cdn.jsdelivr.net/npm/topojson-client@3"></script>
<script src="{{ site.url }}{{ site.baseurl }}/assets/js/footprints-map.js"></script>

{% if site.posts.size > 0 %}
<div class="section-card" markdown="0">
{% for post in site.posts %}
<div class="news-item" style="padding: 1rem 0; border-bottom: 1px solid var(--border-color);">
<span class="news-date">{{ post.date | date: "%b %-d, %Y" }}</span><br>
<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" style="font-weight: 600;">{{ post.title }}</a>
</div>
{% endfor %}
</div>
{% else %}
<p class="text-muted">No blog posts yet.</p>
{% endif %}
