---
layout: single
permalink: /2027/
title: "Workshop on Artificial Intelligence for Scientific Publications (WASP) 2027"
excerpt: "The fifth edition of WASP, co-located with NAACL 2027."
sidebar:
  nav: "sidebar2027"
header:
  overlay_color: "#000"
  overlay_filter: "0.35"
  overlay_image: /assets/2027/san-francisco.jpg
  caption: "Photo: Lightandtruth ([Wikimedia Commons](https://commons.wikimedia.org/wiki/File:San_Francisco_from_the_Marin_Headlands_in_August_2022.jpg), [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/))"
  actions:
    - label: '<i class="fas fa-map-marker-alt"></i>San Francisco · NAACL 2027'
      url: https://2027.naacl.org/
    - label: '<i class="far fa-calendar-alt"></i>June 1–5, 2027'
      url: /2027/important_dates
    - label: '<i class="fas fa-file-alt"></i>Call for Papers'
      url: /2027/call_for_papers
---

<style>
  /* Taller header, framed on the skyline and the bridge deck rather than the middle of the photo. */
  .page__hero--overlay { padding: 5em 0; background-position: center 35%; }
</style>

We are delighted to announce that the fifth edition of WASP will be held at NAACL 2027, the Annual Conference of the Nations of the Americas Chapter of the Association for Computational Linguistics. The workshop will be held in person; the exact date will be announced by the conference.

How can machines read, extract, and structure the knowledge held in the scientific literature? WASP brings the NLP and AI community together around that question, from scientific named-entity recognition and citation mining to summarisation, reproducibility analysis, and the responsible use of large language models in scholarly publishing.

## Latest news

<ul class="news">
  {%- for n in site.data.wasp2027_news %}
  <li class="news__item"><span class="news__date">{{ n.date }}</span><span class="news__text">{{ n.text | markdownify | remove: "<p>" | remove: "</p>" | strip }}</span></li>
  {%- endfor %}
</ul>

## Call for papers

WASP 2027 invites long and short papers across AI for scientific publishing, with a sharpened focus this year on **interpretable and explainable scientific reasoning**. The workshop is held in person in San Francisco.

- [Call for Papers](call_for_papers): themes and topics of interest
- [Important Dates](important_dates): submission and shared task deadlines
- [Submission & Policies](submission): paper types, formatting and review

WASP 2027 will also host a shared task; details will be announced soon.

## Organizers

- [Atilla Kaan Alkan](https://ui.adsabs.harvard.edu/about/team/team/aalkan.html), Center for Astrophysics \| Harvard & Smithsonian, USA
- [Alberto Accomazzi](https://ui.adsabs.harvard.edu/about/team/team/aaccomazzi.html), Center for Astrophysics \| Harvard & Smithsonian, USA
- [Tirthankar Ghosal](https://www.ornl.gov/staff-profile/tirthankar-ghosal), Oak Ridge National Laboratory, USA
- [Felix Grezes](https://ui.adsabs.harvard.edu/about/team/team/fgrezes.html), Center for Astrophysics \| Harvard & Smithsonian, USA
- [Kelly Lockhart](https://ui.adsabs.harvard.edu/about/team/team/klockhart.html), Center for Astrophysics \| Harvard & Smithsonian, USA

## Previous editions

{% include editions.html exclude=2027 %}

## Contact

For enquiries, contact Atilla Kaan Alkan at [atilla.alkan@cfa.harvard.edu](mailto:atilla.alkan@cfa.harvard.edu).
