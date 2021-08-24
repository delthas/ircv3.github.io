---
layout: page
title: Clients
meta-description: IRCv3 Client Support. This page lists the IRC clients compatible with and supporting IRCv3 features.
data-source-filename: sw_clients.yml
page-header: >
  IRCv3 Client Support
---
{% include software_intro.html %}

<div class="irc-sw-list flexy-list">
{% for type in site.data.sw_clients %}
<a href="#{{ type.name | slugify }}">{{ type.name }}</a>
{% endfor %}
</div>

{% for type in site.data.sw_clients %}
{% include software_list.html %}
{% endfor %}
