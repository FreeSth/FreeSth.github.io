---
layout: default
---

<div class="small-container">
  {% for post in site.categories["公告"] %}
    <a href="{{ site.baseurl }}{{ post.url }}" class="article-link">
      <article class="article-excerpt">
        <div>
          <h1>{{ post.title }}</h1>
          <time>{{ post.date | date: "%B %e, %Y" }}</time>
          <p>
            {{ post.excerpt }}
          </p>
        </div>
        <div class="article-image">
          <img src="{{ post.image }}" alt="{{post.title}}">
        </div>
      </article>
    </a>
  {% endfor %}
</div>