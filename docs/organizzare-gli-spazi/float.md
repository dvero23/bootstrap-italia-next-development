---
layout: docs
title: Float
description: Gestisci i float di qualsiasi elemento con le classi apposite.
group: organizzare-gli-spazi
toc: true
---

Queste classi permettono di dare a un elemento la [proprietà `float`](https://developer.mozilla.org/en-US/docs/Web/CSS/float)
a sinistra, a destra o di disabilitarlo.

`!important` è incluso nelle classi per evitare problemi di ereditarietà pregressa.

## Classi

Attiva o disattiva il `float` con le seguenti classi:

{% capture example %}

<div class="float-start">Esempio di float a sinistra per tutte le dimensioni</div><br>
<div class="float-end">Esempio di float a destra per tutte le dimensioni</div><br>
<div class="float-none">Float disattivo per tutte le dimensioni</div>
{% endcapture %}{% include example.html content=example %}

## Responsive

Esistono variazioni delle classi `float` per i vari tipi di dimensione dello schermo.

{% capture example %}

<div class="float-sm-start">Esempio di float a sinistra per dimensioni SM (small) o maggiori.</div><br>
<div class="float-md-start">Esempio di float a sinistra per dimensioni MD (medium) o maggiori.</div><br>
<div class="float-lg-start">Esempio di float a sinistra per dimensioni LG (large)  o maggiori.</div><br>
<div class="float-xl-start">Esempio di float a sinistra per dimensioni XL (extra-large) o maggiori.</div><br>
<div class="float-xxl-start">Esempio di float a sinistra per dimensioni XXL (extra-extra-large) o maggiori.</div><br>
{% endcapture %}{% include example.html content=example %}

Di seguito l'elenco completo delle classi a disposizione:

{% for bp in site.data.breakpoints %}

- `.float{{ bp.abbr }}-start`
- `.float{{ bp.abbr }}-end`
- `.float{{ bp.abbr }}-none`{% endfor %}
