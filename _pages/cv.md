---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Employment

<div class="cv-entry" markdown="1">
<div class="cv-entry__head"><strong>Postdoctoral Researcher</strong><span class="cv-entry__date">Feb 2026 – Present</span></div>
<div class="cv-entry__where">EPFL, Lausanne, Switzerland</div>

* Beam-beam and optics studies for the Future Circular Collider (FCC).
</div>

<div class="cv-entry" markdown="1">
<div class="cv-entry__head"><strong>Senior Applied Fellow</strong><span class="cv-entry__date">Mar 2023 – Jan 2026</span></div>
<div class="cv-entry__where">CERN, Geneva, Switzerland</div>

* Assessing the beam performance capabilities and limitations of the accelerator complex within the Physics Beyond Colliders (PBC) study.
  * Studies for optimizing high-intensity beam performance of the PSB, PS, and SPS.
  * Optics measurement and correction, loss minimization, resonance compensation, space charge, instabilities.
* Teaching assistant in CAS, JUAS and EUROLABS.
</div>

<div class="cv-entry" markdown="1">
<div class="cv-entry__head"><strong>Doctoral Student</strong><span class="cv-entry__date">Mar 2020 – Feb 2023</span></div>
<div class="cv-entry__where">CERN, Geneva, Switzerland</div>

* Optics measurement and correction at PSB injection.
* Development of a k-modulation GUI application in Python for the PSB operation.
* Optimization of the transverse beam profiles shape and reconstruction.
* Space charge effects near the half-integer resonance.
</div>

<div class="cv-entry" markdown="1">
<div class="cv-entry__head"><strong>Technical Student</strong><span class="cv-entry__date">Aug 2018 – Jul 2019</span></div>
<div class="cv-entry__where">CERN, Geneva, Switzerland</div>

* Emittance & dispersion measurements and emittance deconvolution algorithms in the PSB.
</div>

## Education

<div class="cv-entry" markdown="1">
<div class="cv-entry__head"><strong>PhD in Accelerator Physics</strong><span class="cv-entry__date">2020 – 2023</span></div>
<div class="cv-entry__where">Goethe University Frankfurt</div>

Thesis: [*Optimization of the High Brightness Beam Performance of the CERN PSB with H- Injection*](https://cds.cern.ch/record/2887279)
</div>

<div class="cv-entry" markdown="1">
<div class="cv-entry__head"><strong>Integrated Master in Applied Physics</strong><span class="cv-entry__date">2014 – 2019</span></div>
<div class="cv-entry__where">National Technical University of Athens</div>

Thesis: [*Transverse Emittance and Brightness Studies in the CERN PSB*](https://indico.cern.ch/event/849052/contributions/3567761/attachments/1910604/3166227/semfe_thesis_tprebibaj_final.pdf)
</div>

## Specialized Training

<div class="cv-entry">
<div class="cv-entry__head"><strong>CERN Accelerator School (CAS), <em>Advanced Accelerator Physics</em></strong><span class="cv-entry__date">Nov 2022</span></div>
<div class="cv-entry__where">Sevrier, France</div>
</div>

<div class="cv-entry">
<div class="cv-entry__head"><strong>US Particle Accelerator School (USPAS), <em>Beam Physics with Intense Space Charge</em></strong><span class="cv-entry__date">Jan 2020</span></div>
<div class="cv-entry__where">San Diego, CA, USA</div>
</div>

<div class="cv-entry">
<div class="cv-entry__head"><strong>Joint Universities Accelerator School (JUAS), <em>The Science of Particle Accelerators</em></strong><span class="cv-entry__date">Jan 2019</span></div>
<div class="cv-entry__where">European Scientific Institute (ESI), Archamps, France</div>
</div>

## Teaching

{% assign courses = site.teaching | sort: "order" %}
{% for c in courses %}
<div class="cv-entry">
<div class="cv-entry__head"><strong><a href="{{ base_path }}{{ c.url }}">{{ c.title }}</a></strong><span class="cv-entry__date">{% for e in c.editions reversed %}{{ e.year }}{% unless forloop.last %}, {% endunless %}{% endfor %}</span></div>
<div class="cv-entry__where">{{ c.venue }}{% if c.course %} · <em>{{ c.course }}</em>{% endif %}</div>
</div>
{% endfor %}

## Selected Talks

{% assign recent_talks = site.talks | reverse %}
{% for t in recent_talks limit: 5 %}
<div class="cv-entry">
<div class="cv-entry__head"><strong><a href="{% if t.link %}{{ t.link }}{% else %}{{ base_path }}{{ t.url }}{% endif %}">{{ t.title }}</a></strong><span class="cv-entry__date">{{ t.date | date: "%b %Y" }}</span></div>
<div class="cv-entry__where">{{ t.venue }}, {{ t.location }}</div>
</div>
{% endfor %}
<p><a href="{{ base_path }}/talks/">All talks →</a></p>

## Skills

<dl class="cv-skills">
  <dt>Programming &amp; Data Analysis</dt><dd>Python · MATLAB · Java</dd>
  <dt>Data Systems</dt><dd>Git · NXCALS · LSA · PyJAPC · UCAP</dd>
  <dt>Simulation Software</dt><dd>Xsuite · PyOrbit · MAD-X</dd>
  <dt>Professional</dt><dd>Accelerator operation &amp; optimization · Scientific reporting · Mentoring &amp; supervising</dd>
</dl>
