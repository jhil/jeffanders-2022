---
layout: post
category: list
title: "Angel Investing"
date: 2022-01-01
thumbnail: circle-multiple
---

Emily and I have backed a few startups with very small checks. We like helping as advisors and supporting fellow founders. <a href="mailto:jahilnbrand@gmail.com">Contact us</a> if you're raising!

<ul class="card-grid card-grid-compact">
	{% for investing in site.data.investing %}
	{% if investing.type contains "angel" %}
		<li class="compact-card compact-card-medium"><a href="{{ investing.link }}" target="_blank">
			<img src="{{ investing.image }}" alt="{{ investing.company }} logo">
			<h3>{{ investing.company }}</h3>
			<p class="card-secondary">{{ investing.round }}</p>
		</a></li>
	{% endif %}
	{% endfor %}
</ul>
