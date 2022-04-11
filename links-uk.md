---
lang: uk
pageid: links
title: Посилання та ресурси
description: Збір корисних посилань і ресурсів

---
{% assign cantons = site.data.links.cantons | sort: page.lang %}
# {{ page.title }}

# Кантональна допомога Україні
Контакти та інформація різних кантонів

{% for item in cantons %}[{{ item.canton }}](#{{ item.canton }}) - {% endfor %}
{% for item in cantons %}
### [{{ item.uk }}]({{ item.url1 }}) - **{{ item.canton }}**
{% if item.uk2 %}{{ item.uk2 }}{% endif %}
- Гаряча лінія: **{{ item.hotline }}** 
- Електронна пошта: [{{ item.mail }}](mailto:{{ item.mail }})
- Джерело: [www]({{ item.url2 }})
{% endfor %}





