---
layout: page
permalink: /play
title: Play
description: interests and hobbies
nav: true
display_categories: [Fun]
horizontal: false
---
<div class="play">
  {% if site.enable_play_categories and page.display_categories %}
  <!-- Display categorized play -->
    {% for category in page.display_categories %}
      <h2 class="category">{{category}}</h2>
      {% assign categorized_play = site.play | where: "category", category %}
      {% assign sorted_play = categorized_play | sort: "importance" %}
      <!-- Generate cards for each play -->
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-2">
          {% for play in sorted_play %}
            {% include play_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {% for play in sorted_play %}
            {% include play.html %}
          {% endfor %}
        </div>
      {% endif %}
    {% endfor %}

  {% else %}
  <!-- Display play without categories -->
    {% assign sorted_play = site.play | sort: "importance" %}
    <!-- Generate cards for each play -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for play in sorted_play %}
          {% include play_horizontal.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for play in sorted_play %}
          {% include play.html %}
        {% endfor %}
      </div>
    {% endif %}

  {% endif %}

</div>