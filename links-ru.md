---
lang: ru
pageid: links
title: Ссылки и ресурсы
description: Каталог ссылок и ресурсов

---
{% assign cantons = site.data.links.cantons | sort: page.lang %}
# {{ page.title }}

## Кантонал Украина Справка и информация
Контакты и информация кантонов

{% for item in cantons %}[{{ item.canton }}](#{{ item.canton }}) - {% endfor %}
{% for item in cantons %}
### [{{ item.ru }}]({{ item.url1 }}) - **{{ item.canton }}**
{% if item.ru2 %}{{ item.ru2 }}{% endif %}
- Hotline: **{{ item.hotline }}** 
- Mail: [{{ item.mail }}](mailto:{{ item.mail }})
- Source: [www]({{ item.url2 }})
{% endfor %}






