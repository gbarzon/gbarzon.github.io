---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

Here you can find the list of all my pubblications and a network representing my work and collaborators; the color of each node specifies what it represents: <span style="color:#9BA1A6">co-authors</span>, <span style="color:#dbbb2a">preprints</span> or <span style="color:#9e1910">journal articles</span>. Hover and click on each node for more information, or drag them around to change the network's shape.
<iframe src="/collab_net/network.html" height="300" width="100%" style="border: none"></iframe>

{% for post in site.publications reversed %}
  {% include archive-single-publication.html %}
{% endfor %}
