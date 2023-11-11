---
layout: page
---

<h3>Latest Posts</h3>

<style>
  ul {
      list-style-type: none; /* Remove default bullets */
      padding: 0; /* Remove default padding */
  }
</style>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        <time datetime="{{ post.date | date_to_xmlschema }}">
          {%- assign date_format = "%b %-d, %Y" -%}
          [{{ post.date | date: date_format }}]
        </time>
        {{ post.title }}
      </a>
    </li>
  {% endfor %}
</ul>
