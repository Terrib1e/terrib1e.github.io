---
layout: default
title: Blog
description: 
permalink: /blog/
---
<h1 class="page-heading">Blog</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        
        <h2 id="post-index">
         <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>