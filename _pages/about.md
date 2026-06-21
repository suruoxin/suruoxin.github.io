---
title: "About"
layout: gridlay
permalink: /about/
---

## About

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ site.photo }}" class="pi-photo" alt="{{ site.name }}" loading="lazy">
<div>
<h3 class="pi-name">{{ site.name }}</h3>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.url }}{{ site.baseurl }}/{{ site.links.cv }}" class="icon-link" title="CV"><i class="ai ai-cv"></i></a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
{% if site.links.orcid and site.links.orcid != "" %}<a href="{{ site.links.orcid }}" class="icon-link" title="ORCID"><i class="ai ai-orcid"></i></a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>{% endif %}
{% if site.links.researchgate and site.links.researchgate != "" %}<a href="{{ site.links.researchgate }}" class="icon-link" title="ResearchGate"><i class="ai ai-researchgate"></i></a>{% endif %}
</div>
{% if site.data.pi[0].education %}
<ul style="margin-top: var(--space-4);">
{% for education in site.data.pi[0].education %}
<li>{{ education | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
{% endif %}
</div>
</div>
</div>

{% if site.data.grants %}
<div class="section-card">
<h3>Work Experience</h3>
<ul>
<li>(2023 - now) Researcher, Vrije Universiteit Brussel, Brussels, Belgium</li>
<li>(2022 - 2023) Privacy Counsel (secondee), Apple Electronics Products Commerce, Beijing, China</li>
<li>(2021 - 2023) Lawyer, Junhe LLP, Beijing, China</li>
<li>(2020) Legal Assistant, Grandall Law Firm, Zhengzhou, China</li>
<li>(2016 - 2017) Barista, Caicai Cafe, Wuhan, China</li>
</ul>
</div>
{% endif %}

{% if site.data.awards %}
<div class="section-card">
<h3>Research Grants</h3>
<ul>
<li>(2026) The 10th Asian Privacy Scholars Network (APSN) Conference Travel Grant, HKD 5,000</li>
</ul>
</div>
{% endif %}

{% if site.data.people %}
<div class="section-card">
<h3>Honors and Awards</h3>
<ul>
<li>(2025) Top Policy Provocation Paper Award, Privacy Law Scholars Conference (PLSC) – Europe 2025, Leiden, The Netherlands</li>
<li>(2020) Eagle Support Project Scholarship for Advanced Legal Studies, Zhongnan University of Economics and Law (ZUEL)</li>
<li>(2020) Outstanding Undergraduate Award, ZUEL</li>
<li>(2020) Outstanding Undergraduate Thesis Award, ZUEL</li>
<li>(2019) International Exchange Programme Scholarship for Outstanding Undergraduates, China Scholarship Council</li>
<li>(2018) Bank of China Scholarship, Bank of China & ZUEL</li>
<li>(2017 - 2019) Second-Class & Third-Class University Scholarships, ZUEL</li>
<li>(2017) First Prize (Team), University Volleyball Competition, ZUEL</li>
</ul>
</div>
{% endif %}
