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

Below you can find the list of all my publications and a network representing my work. The color of each node specifies if it represents co-authors, preprints or journal articles. Click on a node for more information.
<iframe src="/collab_net/network.html" height="400" width="100%" style="border: none"></iframe>

{% for post in site.publications reversed %}
  {% include archive-single-publication.html %}
{% endfor %}
