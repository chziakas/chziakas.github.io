---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Bio

I am a final-year [**MSCA Doctoral Fellow**](https://marie-sklodowska-curie-actions.ec.europa.eu/) at [**Imperial College London**](https://www.imperial.ac.uk/), advised by [**Prof. Alessandra Russo**](https://www.doc.ic.ac.uk/~acr/) and [**Prof. Joey Bose**](https://scholar.google.com/citations?user=ybPyI7IAAAAJ&hl=en). My research focuses on the **generalization**, **test-time adaptation**, and **evaluation** of foundation **generative models**.

Currently, I am a Research Intern at [**Microsoft Research AI Frontiers**](https://www.microsoft.com/en-us/research/lab/ai-frontiers/) in New York, hosted by [**Siddhartha Sen**](https://www.microsoft.com/en-us/research/people/sidsen/) and [**John Langford**](https://www.microsoft.com/en-us/research/people/jcl/). I collaborated with [**Google DeepMind**](https://deepmind.google/) on benchmarking LLMs on hard STEM tasks. Previously, I worked at [**Microsoft AI**](https://www.microsoft.com/en-us/ai) on post-training [**Copilot**](https://www.microsoft.com/en-us/microsoft-365/copilot) for tool use and reasoning.

Before pursuing a PhD in AI, I co-founded [**Athina AI (YC W23)**](https://www.athina.ai/), an LLM observability startup. I also hold an MSc in Data Science from [**TU Munich**](https://www.tum.de/), where my thesis on neural temporal point processes was supervised by [**Prof. Stephan Günnemann**](https://scholar.google.com/citations?user=npqoAWwAAAAJ&hl=de) and hosted at [**BMW**](https://www.bmwgroup.com/).

I co-organize the [**ICARL Seminar**](https://icarl.doc.ic.ac.uk/seminar-series) at Imperial and am a mentor at [**SPAR**](https://sparai.org/). Please feel free to reach out if you share similar research interests or would like to discuss transitioning from the startup world to a PhD.




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


