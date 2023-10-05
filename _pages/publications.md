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

<ul>
{% for post in site.publications reversed %}
  {% if post %}
    {% include publication.html %}
  {% endif %}
{% endfor %}
</ul>