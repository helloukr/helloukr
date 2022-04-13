---
lang: de
pageid: links
title: Links & Resourcen
description: Verzeichnis von Links und Resourcen

---
{% assign cantons = site.data.links.cantons | sort: page.lang %}
# {{ page.title }}

## Kantonale Ukraine Hilfe
Kontakte, Informationen, sowie private Hilfsangebote nach Kanton

<table>
<tr>
    <th>Kanton</th>
    <th>Behörden</th>
    <th>Private Angebote</th>
</tr>
{% for item in cantons -%}
<tr>
    <td>
        {{ item.canton }}
        <br/>
        <b>{{ item.de }}</b>
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
