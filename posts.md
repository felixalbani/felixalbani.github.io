---
layout: posts
title: "Felix Albani - Posts"
image: "/assets/images/horse_jumping_ai.png"
---

# Posts

<ul class="post-list p-3 pl-5 pr-5 bg-gray-100 rounded-lg mb-5">
  {% for post in site.posts %}
    <li>     
    <div class="post">
        <ul class="flex h-12 place-items-center">
        <li class="pr-4 text-gray-500 post-meta">{{post.date | date: "%b %d, %Y"}}</li>
        {% if post.substack != "" %}
          <li class="mr-4">
          <a href="{{ post.substack }}" target="_blank" alt="Substack"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24"><path fill="#aaaaaa" d="M22.539 8.242H1.46V5.406h21.08v2.836zM1.46 10.812V24L12 18.11L22.54 24V10.812H1.46zM22.54 0H1.46v2.836h21.08V0z"/></svg></a>
          </li>
        {% endif %}
      </ul>
      <div class="pt-3" ><a href="{{ post.url }}" target="_self" > <span class="post-title">{{ post.title }}</span></a></div>      
      <div class="pt-3">
          <a href="{{ post.url }}" target="_self"><span class="post-description">{{ post.description }}</span></a>
      </div>   
      <div class="pt-3">
        <a href="{{ post.url }}" target="_self"><span class="post-action">Read article ></span></a>
      </div>   
      </div>
    </li>
  {% endfor %}
</ul>
