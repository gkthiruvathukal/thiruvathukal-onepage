---
title: "publications"
bg: pgreen
color: black
fa-icon: book
---

## Publications

Virtually all of my publications can be found in my university's Digital Commons site at [works.bepress.com/gkthiruvathukal](https://works.bepress.com/gkthiruvathukal/).

### CV

Here is a link to my <a href="https://ndownloader.figshare.com/files/10204851">CV</a>, if you require something more formal.

{% assign ecommons = site.data.ecommons %}
{% assign pubtypes = site.data.pubtypes %}

{% for item in pubtypes.items %}
### {{ item.text }}

{% for paper in ecommons %}
{% if paper.document_type == item.type %}

{{ paper.authors }}, *{{ paper.title }}*, [{{ paper.front_end_url }}]({{ paper.front_end_url }})

{% endif %}
{% endfor %}

{% endfor %}

