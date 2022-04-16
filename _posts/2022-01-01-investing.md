---
layout: post
category: list
title: "Investing"
date: 2022-01-01
thumbnail: circle-multiple
---

## Angel

Emily and I have angel invested small checks in a few startups. We like adding value as advisors and generally being there to support founders. <a href="mailto:jahilnbrand@gmail.com">Contact us</a> if you're raising!

<ul class="card-grid card-grid-compact">
	{% for investing in site.data.investing %}
	{% if investing.type contains "angel" %}
		<li class="compact-card compact-card-medium"><a href="{{ investing.link }}">
			<img src="{{ investing.image }}" alt="{{ investing.company }} logo">
			<h3>{{ investing.company }}</h3>
			<p class="card-secondary">{{ investing.round }}</p>
		</a></li>
	{% endif %}
	{% endfor %}
</ul>

## Crowdfunding

<ul class="card-grid card-grid-compact">
	{% for investing in site.data.investing %}
	{% if investing.type contains "crowdfunding" %}
		<li class="compact-card compact-card-medium"><a href="{{ investing.link }}">
			<img src="{{ investing.image }}" alt="{{ investing.company }} logo">
			<h3>{{ investing.company }}</h3>
		</a></li>
	{% endif %}
	{% endfor %}
</ul>

Equities, cryptocurrencies, and alternatives breakdowns coming soon.
