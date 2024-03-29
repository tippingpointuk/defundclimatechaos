---
layout: page
image: /assets/images/og-image.png
blocks:
  - map: false
    text: ''
    id: ''
    buttons: []
    decoration: ''
    background_image: ''
  - text: >-
      # Events & Actions


      {% assign protest = site.actions | where: "future", 1 | where:
      "event_type", "Protest" %}

      {% assign films = site.actions | where: "future", 1 | where: "event_type",
      "Film" %}

      {% assign whildwinds = site.actions | where: "future", 1 | where:
      "event_type", "Whirlwind moment / Mass Mobilisation" %}

      {% assign meetings = site.actions | where: "future", 1 | where:
      "event_type", "Meeting" %}

      {% assign events = meetings | concat: whildwinds | concat: films | concat:
      protest  %}

      {% include events-gallery.html date_field='start_date' summary=true %}


      # Trainings


      {% assign events = site.actions | where: "future", 1 | where:
      "event_type", "Training" %}

      {% include events-gallery.html date_field='start_date' summary=true
      image=false  %}
    map: false
    id: ''
    buttons: []
    decoration: ''
    background_image: ''
  - map: false
    text: >-
      # #StopEACOP


      French oil giant Total and the China National Offshore Oil Corporation are
      on the cusp of building a massive crude oil pipeline right through the
      heart of Africa – displacing communities, endangering wildlife and tipping
      the world closer to full-blown climate catastrophe.


      Building the longest heated oil pipeline in the world is risky work, and
      Total can’t do it alone. They are seeking insurance and funding from some
      of the world’s largest insurance companies and banks to get this project
      off the ground.
    id: stopeacop
    buttons:
      - target: 'https://actionnetwork.org/forms/take-regular-action-to-stopeacop-2'
        image: ''
        new_tab: true
        text: Take Action
      - text: Pass a Trade Union Motion
        target: '#StopEACOPtu'
        image: ''
        new_tab: false
    decoration: ''
    background_image: ''
  - map: false
    text: >-
      ## Trade Union Motion


      If you are part of a Trade Union, you can support the #StopEACOP campaign
      by passing this motion at your local branch.


      {% include motions.html limit=1 %}
    id: StopEACOPtu
    buttons: []
    decoration: ''
    background_image: ''
  - map: false
    text: >-
      ## Money is fuelling climate chaos. Climate justice means keeping fossil
      fuels in the ground. We can support struggles across the globe by cutting
      off the money and insurance for new projects.


      {% include an-email-only-form.html
      endpoint="https://actionnetwork.org/api/v2/petitions/e0c7e2f4-925f-448c-9558-57c1997b5408/signatures"
      jump="actions" %}
    id: ''
    buttons: []
    decoration: ''
    background_image: ''
  - buttons: []
    text: >-
      # Resources


      Want to keep organising to #DefundClimateChaos beyond today.   Here's all
      the resources you’ll need to keep taking action throughout COP26 and
      beyond


      {% include resources.html %}
    decoration: ''
    map: false
    background_image: ''
    id: ''
  - buttons: []
    text: |-
      # Find out more

      Some frequently asked questions and answers

      {% include accordion.html data=site.data.faqs %}
    decoration: ''
    map: false
    background_image: ''
    id: faqs
credits: ''
invert: odd
title: Act
tags: []
permalink: act
summary: ''
share:
  whatsapp: ''
  text: ''
  tweet: ''
logo: ''
logo_square: ''
header:
  text: ''
  buttons: []
  border_bottom:
    image: ''
    reflect: false
menu:
  header:
    title: Take Action
    weight: 1
_template: block_layout
---

