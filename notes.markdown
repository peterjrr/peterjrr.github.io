---
title: Notes
date: 2021-02-15 07:41:00 Z
layout: default
---

<section class="notes-index">
  <ul>
  {% for note in site.notes %}
  <li class="notes-index-item">
    <h2 class="notes-index-title">
      <a href="{{ note.url }}">
        {{ note.title }}
      </a>
    </h2>
    <p class="notes-index-date"><timedatetime="{{ note.date | date: "%Y-%m-%d" }}">{{ note.date | date_to_long_string }}</time></p>
    <!-- {{ note.content }} -->
  </li>
{% endfor %}
</ul>
</section>
