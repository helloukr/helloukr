---
lang: de
pageid: links
title: Links & Resourcen
description: Verzeichnis von Links und Resourcen

---
{% assign cantons = site.data.links.cantons | sort: page.lang %}
# {{ page.title }}

## Kantonale Ukraine Hilfe
Kontakte und Informationen der Kantone

{% for item in cantons %}[{{ item.canton }}](#{{ item.canton }}) - {% endfor %}
{% for item in cantons %}
<a id="{{ item.canton }}"></a>
### [{{ item.de }}]({{ item.url1 }}) - **{{ item.canton }}**
{% if item.de2 %}{{ item.de2 }}{% endif %}
- Hotline: **{{ item.hotline }}** 
- Mail: [{{ item.mail }}](mailto:{{ item.mail }})
- Source: [www]({{ item.url2 }})
{% endfor %}



