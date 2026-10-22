---
layout: page
title: Article
page_style: academic-doc
---

这里收录了随笔、读书笔记、诗歌与小说。点击标题即可阅读全文。
{: .message }

<div class="article-collection">
  {% assign articles = site.categories.article | sort: "date" | reverse %}
  {% assign current_year = "" %}
  {% for post in articles %}
    {% assign post_year = post.date | date: "%Y" %}
    {% if post_year != current_year %}
      {% unless forloop.first %}</ul></section>{% endunless %}
      <section class="article-year">
        <h2>{{ post_year }}</h2>
        <ul class="article-list">
      {% assign current_year = post_year %}
    {% endif %}
    <li>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y.%m.%d" }}</time>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="article-category">{{ post.article_category }}</span>
    </li>
  {% endfor %}
  {% if articles.size > 0 %}</ul></section>{% endif %}
</div>
