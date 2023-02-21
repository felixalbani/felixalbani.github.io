---
layout: default
title: "Felix Albani - Posts"
---

# Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
     <a class="post-link" href="{{ post.url }}">
      <div class="post-item-header">
            <p class="post-item-meta">
             <span class="post-item-date">{{page.date | date: "%b %d, %Y"}}</span>
            </p>
            <h2 class="post-item-title">{{ post.title }}</h2>
        </div>
        <div class="post-item-description">
            <p>
               {{ post.description }}
            </p>
        </div>      
      </a>
    </li>
  {% endfor %}
</ul>
