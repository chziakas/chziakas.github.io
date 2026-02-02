---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Bio

I am a [**Marie Skłodowska-Curie Doctoral Fellow**](https://marie-sklodowska-curie-actions.ec.europa.eu/) at [**Imperial College London**](https://www.imperial.ac.uk/), advised by [**Prof. Alessandra Russo**](https://www.doc.ic.ac.uk/~acr/). My research interests lie in **generalist agents**, **world models**, and **AI safety**. Previously, I worked at [**Microsoft AI**](https://www.microsoft.com/en-us/ai) on post-training [**Microsoft 365 Copilot**](https://www.microsoft.com/en-us/microsoft-365/copilot) for tool use and reasoning.

Before pursuing a PhD in AI, I co-founded [**Athina AI (YC W23)**](https://www.athina.ai/), an LLM observability startup, and worked in machine learning roles at Turo, BMW, and Amazon. Please feel free to reach out if you share similar research interests or would like to discuss transitioning from the start-up world to a PhD.




<h2>Selected Publications & Preprints</h2>

{% assign selected_pubs = site.publications | where: "selected", true | sort: "weight" %}
{% for post in selected_pubs %}
<p style="margin-bottom: 1rem;">
{% if post.paperurl %}<a href="{{ post.paperurl }}"><b>{{ post.title }}.</b></a>{% else %}<b>{{ post.title }}.</b>{% endif %}<br>
<i>{{ post.authors | replace: "<b>", "<span style='font-weight:600;'>" | replace: "</b>", "</span>" }}.</i><br>
{{ post.venue }}{% unless post.venue contains "202" %}, {{ post.date | date: "%Y" }}{% endunless %}.
</p>
{% endfor %}

<p style="font-size:0.85em; margin-top:0.5rem;">
  For a full list, please visit <a href="/publications/">Publications & Preprints</a> page.
</p>
<p style="font-size:0.85em;">
  &#42; indicates equal first authorship.
</p>


