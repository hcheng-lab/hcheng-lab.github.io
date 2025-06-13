---
title: "Cheng Lab - Publications"
layout: gridlay
excerpt: "Cheng Lab -- Publications."
sitemap: false
permalink: /publications/
---

<script async src="https://badge.dimensions.ai/badge.js" charset="utf-8"></script>


# Publications

## Group highlights

**At the end of this page, you can find the [full list of publications](#full-list-of-publications). See also <a href="https://scholar.google.com/citations?user=Vff5EiwAAAAJ" target="_blank">Google Scholar</a>.**


(<sup>&#8224;</sup> for corresponding authors; bold font for lab members)


<ul>
{% for publi in site.data.seclectpub %}
<li>
{{ publi.authors }} ({{ publi.year }}) {{ publi.title }}. <a href="{{ publi.url }}">{{ publi.display }}</a>.
[PMID: <a href="https://www.ncbi.nlm.nih.gov/pubmed/{{ publi.pmid }}">{{ publi.pmid }}</a>]
<span style="display:inline-block;" class="__dimensions_badge_embed__" data-legend="never" data-pmid="{{ publi.pmid }}" data-style="small_rectangle"></span>
<!--
[<a href="https://badge.dimensions.ai/details/pmid/{{ publi.pmid }}">Citations</a>]
-->
</li>
{% endfor %}
</ul>

## Full List of publications

<ul>
{% for publi in site.data.publist %}
<li>
{{ publi.authors }} ({{ publi.year }}) {{ publi.title }}. <a href="{{ publi.url }}">{{ publi.display }}</a>.
[PMID: <a href="https://www.ncbi.nlm.nih.gov/pubmed/{{ publi.pmid }}">{{ publi.pmid }}</a>]
<span style="display:inline-block;" class="__dimensions_badge_embed__" data-legend="never" data-pmid="{{ publi.pmid }}" data-style="small_rectangle"></span>
<!--
[<a href="https://badge.dimensions.ai/details/pmid/{{ publi.pmid }}">Citations</a>]
-->
</li>
{% endfor %}
</ul>
