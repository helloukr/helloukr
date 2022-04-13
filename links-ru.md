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


<table>
<tr>
    <th>Кантон</th>
    <th>официальная информация</th>
    <th>Частные предложения</th>
</tr>
{% for item in cantons -%}
<tr>
    <td>
        {{ item.canton }}
        <br/>
        <b>{{ item.ru }}</b>
    </td>
    <td>
        <ul>
            <li>Hotline: <a href="tel:{{ item.hotline  | remove: ' ' }}">{{ item.hotline }}</a> </li>
            <li>Mail: <a href="mailto:{{ item.mail }}">{{ item.mail }}</a> </li>
            <li>Source: <a href="{{ item.url1 }}">www</a> </li>
        </ul>
    </td>
    <td>
    {% if item.links %}
        <ul>
        {% for link in item.links %} 
            <li><a href="{{ link.url }}">{{ link.name }}</a></li>
        {% endfor %}
        </ul>
    {% endif %}
    </td>
</tr>
{% endfor %}
</table>




