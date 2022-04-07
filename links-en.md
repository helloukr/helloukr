---
lang: en
pageid: links
title: Links & Resources
description: Collection of useful links and resources

---
{% assign cantons = site.data.links.cantons | sort: page.lang %}
# {{ page.title }}

# Cantonal Information & Support 
Contacts and information of the cantons

{% for item in cantons %}[{{ item.canton }}](#{{ item.canton }}) - {% endfor %}
{% for item in cantons %}
### [{{ item.en }}]({{ item.url1 }}) - **{{ item.canton }}**
{% if item.en2 %}{{ item.en2 }}{% endif %}
- Hotline: **{{ item.hotline }}** 
- Mail: [{{ item.mail }}](mailto:{{ item.mail }})
- Source: [www]({{ item.url2 }})
{% endfor %}



