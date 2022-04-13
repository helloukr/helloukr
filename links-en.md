---
lang: en
pageid: links
title: Links & Resources
description: Collection of useful links and resources

---
{% assign cantons = site.data.links.cantons | sort: page.lang %}
# {{ page.title }}

# Cantonal Information & Support 
Contacts, information, anf private offers by canton

<table>
<tr>
    <th>Canton</th>
    <th>Authorities</th>
    <th>Private Offers</th>
</tr>
{% for item in cantons -%}
<tr>
    <td>
        {{ item.canton }}
        <br/>
        <b>{{ item.en }}</b>
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
