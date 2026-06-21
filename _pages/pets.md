---
title: "Pets"
layout: gridlay
sitemap: false
permalink: /pets/
---

## Pets 🐾

**A small corner dedicated to my cats and dog, who accompany life beyond academia.**

## Cats

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/team/kibbeling.jpg" class="pi-photo pet-photo" alt="Kibbeling" loading="lazy">
<div>
<h3 class="pi-name">Kibbeling</h3>
<p style="font-style: italic; color: var(--text-secondary);">Content coming soon</p>
</div>
</div>
</div>

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/team/61.jpg" class="pi-photo pet-photo" alt="61" loading="lazy">
<div>
<h3 class="pi-name">61</h3>
<p style="font-style: italic; color: var(--text-secondary);">Content coming soon</p>
</div>
</div>
</div>

{% if site.data.team_members.size > 0 %}
## Current Students and Postdocs

<div class="team-grid">
{% for member in site.data.team_members %}
<div class="team-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" class="team-photo" alt="{{ member.name }}" loading="lazy">
<h4 class="team-name">{{ member.name }}</h4>
<p class="team-info">{{ member.info }}</p>
<div class="team-links">
{% if member.email %}<a href="mailto:{{ member.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>{% endif %}
{% if member.website %}<a href="{{ member.website }}" class="icon-link" title="Website"><i class="fa-solid fa-house"></i></a>{% endif %}
{% if member.scholar %}<a href="{{ member.scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if member.github %}<a href="{{ member.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
</div>
</div>
{% endfor %}
</div>
{% endif %}

## Dog

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/team/chai.jpg" class="pi-photo pet-photo" alt="Chai" loading="lazy">
<div>
<h3 class="pi-name">Chai</h3>
<p style="font-style: italic; color: var(--text-secondary);">Content coming soon</p>
</div>
</div>
</div>
