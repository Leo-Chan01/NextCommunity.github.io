---
layout: default
permalink: /network/
title: Community of programmers and software engineers
---

<h1>
	<a href="/">&uarr;</a>
	Community of programmers and software engineers
</h1>

<p>
Do you want to see yourself here? click [here](https://github.com/BaseMax/NextMaxCommunity) to add your own.
</p>

<style type="text/css">
ul.accounts li {
  float: left;
  width: 100%;
  list-style: none;
  margin-bottom: 10px;
}
ul.accounts li img {
  float: left;
  margin-right: 10px;
}
ul.accounts li div {
  float: left;
  font-size: 20px;
}
ul.accounts ul div * {
  font-size: initial;
}
ul.accounts h4, ul.accounts h5, ul.accounts h6 {
  padding: 0;
  margin: 0;
}
</style>

## List of persons

<ul class="accounts">
{% for network in site.networks %}
  <li>
    <a href="{{ network.url | relative_url }}">
    <img src="https://github.com/{{ network.github }}.png?size=80" width="60">
    <div>
      <h4>{{ network.name }}</h4>
      <h5>{{ network.role }}</h5>
      <h6>{{ network.country}}, {{ network.location}}</h6>
    </div>
  </li>
{% endfor %}
</ul>