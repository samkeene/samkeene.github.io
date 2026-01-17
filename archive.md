---
layout: archive
title: "Blog Posts"
permalink: /archive/
entries_layout: grid
---

<div class="archive">
  {% for post in site.posts %}
    <article class="archive-item">
      <h2 class="entry-title">
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </h2>
      <time datetime="{{ post.date | date_to_xmlschema }}" class="entry-date">{{ post.date | date: "%B %d, %Y" }}</time>
    </article>
  {% endfor %}
</div>
