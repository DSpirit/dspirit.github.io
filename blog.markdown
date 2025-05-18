---
layout: page
title: Blog
permalink: /blog/
---

# Technical Articles & Insights

Below you'll find all my articles on cloud architecture, .NET development, domain-driven design, and more.

<div class="post-list">
  {% for post in site.posts %}
    <article class="post-item">
      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <div class="post-meta">
        {{ post.date | date: "%B %d, %Y" }}
        {% if post.categories.size > 0 %}
          <span class="post-categories">
            {% for category in post.categories %}
              <span class="post-category">{{ category }}</span>
            {% endfor %}
          </span>
        {% endif %}
      </div>
      <div class="post-excerpt">
        {{ post.excerpt }}
      </div>
      <a href="{{ post.url | relative_url }}" class="read-more">Continue reading &rarr;</a>
    </article>
  {% endfor %}
</div>

## Subscribe

Stay up to date with my latest articles and projects:

- Subscribe to my [RSS feed]({{ "/feed.xml" | relative_url }})
- Follow me on [Twitter](https://twitter.com/wendelinniesl)
- Connect with me on [LinkedIn](https://www.linkedin.com/in/wendelin-niesl-676442138/)
