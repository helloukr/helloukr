---
lang: de
pageid: mobile
title: SIM Karten & Mobiltelefonie
tagline: Mobiltelefonie, SIM-Karten und Internet Abos / Verträge
provider:
    - name: Sunrise
      url: https://www.sunrise.ch/en/home
    - name: Salt
      url: https://fiber.salt.ch/en
    - name: Swisscom
      url: https://www.swisscom.ch/en/residential.html
    - name: Provider List
      url: https://www.providerliste.ch/provider/mobile.html
---
# {{ page.title }}

Alle SIM-Karten in der Schweiz müssen mit einem gültigen amtlichen Ausweisdokument (Pass, Personalausweis) registriert sein. Führerscheine werden nicht akzeptiert. Je nach Mobilfunkanbieter können SIM-Karten für den Vertrag mit CHF 40.- belastet werden.

> Sunrise, Swisscom und Salt übernehmen vorübergehend die Kosten für Anrufe in die Ukraine und von der Ukraine in die Schweiz. Das Angebot ist befristet, Termin abklären.

- [Kostenlose Anrufe in die Ukraine](https://www.blick.ch/wirtschaft/anrufe-und-roaming-kostenlos-swisscom-sunrise-und-salt-unterstuetzen-die-ukraine-id17279915.html)

## Telecom / Mobile Anbieter
{% for item in provider %}
- [{{ item.name }}]({{ item.url }})
{% endfor %}


