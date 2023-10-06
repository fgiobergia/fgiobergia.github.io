---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  A list of articles is also available on <u><a href="{{author.googlescholar}}">Google Scholar</a>.</u>
{% endif %}

{% include base_path %}

{% site.publications %}
<ul>
{% for post in site.publications reversed %}
  {% post %}
  {% include publication.html %}
{% endfor %}
</ul>