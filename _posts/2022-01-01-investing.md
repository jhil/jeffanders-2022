---
layout: post
category: list
title: "Investing"
date: 2022-01-01
thumbnail: circle-multiple
---

## Angel

Emily and I have backed a few startups with very small checks. We like helping as advisors and supporting fellow founders. <a href="mailto:jahilnbrand@gmail.com">Contact us</a> if you're raising!

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

## Stocks

Some of the equities we hold and the percent of portfolio. Updated 10/29/2022.

<ul class="card-grid card-grid-compact">
	{% for stock in site.data.stocks %}
		<li class="compact-card compact-card-medium"><a href="https://robinhood.com/stocks/{{ stock.ticker }}">
			<h3 class="stock-company">{{ stock.name }}</h3>
			<span class="card-secondary">{{ stock.percent }}</span>
		</a></li>
	{% endfor %}
</ul>

## Crypto

We're excited about the opportunities in web3 / cryptocurrency and experiment with the technology. Updated 10/29/2022.

<ul class="card-grid card-grid-compact">
	{% for crypto in site.data.cryptos %}
		<li class="compact-card compact-card-medium"><a href="{{ crypto.link }}">
			<img src="/img/investing/{{ crypto.ticker }}.png" alt="{{ crypto.name }} logo">
			<h3 class="stock-company">{{ crypto.name }}</h3>
			<span class="card-secondary">{{ crypto.percent }}</span>
		</a></li>
	{% endfor %}
</ul>



## Crowdfunding

Select crowdfunding projects we've contributed to.

<ul class="card-grid card-grid-compact">
	{% for investing in site.data.investing %}
	{% if investing.type contains "crowdfunding" %}
		<li class="compact-card compact-card-medium"><a href="{{ investing.link }}">
			<img src="{{ investing.image }}" alt="{{ investing.name }} logo">
			<h3>{{ investing.company }}</h3>
		</a></li>
	{% endif %}
	{% endfor %}
</ul>
