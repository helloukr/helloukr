---
lang: en
pageid: index
title: Welcome - Willkommen - Прошу
description: Полезная информация для людей, ищущих защиты от Украины
---
# {{ page.title }}

## Прошу
HelloUkraine.ch дає біженцям з України цінні підказки та поради щодо успішного старту в Швейцарії.

Веб-сайт у вільний час керують волонтери. Зміст ретельно зібраний, але не претендує на актуальність,
фактичну правильність або повність; відповідна гарантія не надається.

- {% for item in site.data.topnav %}[{{ item.uk }}]({{ item.pagebase }}-uk.html){% if forloop.last != true %} - {% endif %}{% endfor %}


## Willkommen
HelloUkraine.ch gibt Flüchtlingen aus der Ukraine wertvolle Hinweise und Tips für einen gelungenen Start in der Schweiz.

Die Webseite wird von Freiwilligen in ihrer Freizeit gemanaged. Die Inhalte sind sorgfältig zusammengestellt, erheben aber
keinen Anspruch auf Aktualität, sachliche Korrektheit oder Vollständigkeit; eine entsprechende Gewähr wird nicht übernommen.

- {% for item in site.data.topnav %}[{{ item.de }}]({{ item.pagebase }}-de.html){% if forloop.last != true %} - {% endif %}{% endfor %}



## Welcome
HelloUkraine.ch gives refugees from Ukraine valuable hints and tips for a successful start in Switzerland.

The website is managed by volunteers in their spare time. The contents are carefully compiled, but do not claim
to be up-to-date, factually correct or complete; no corresponding guarantee is given.

- {% for item in site.data.topnav %}[{{ item.en }}]({{ item.pagebase }}-en.html){% if forloop.last != true %} - {% endif %}{% endfor %}

