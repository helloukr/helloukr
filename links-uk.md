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

<table>
<tr>
    <th>Кантон</th>
    <th>Офіційна інформація</th>
    <th>Приватні пропозиції</th>
</tr>
{% for item in cantons -%}
<tr>
    <td>
        {{ item.canton }}
        <br/>
        <b>{{ item.uk }}</b>
    </td>
    <td>
        <ul>
            <li>Гаряча лінія: <a href="tel:{{ item.hotline  | remove: ' ' }}">{{ item.hotline }}</a> </li>
            <li>Електронна пошта: <a href="mailto:{{ item.mail }}">{{ item.mail }}</a> </li>
            <li>Джерело: <a href="{{ item.url1 }}">www</a> </li>
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




