---
layout: page
title: 个人博客
subtitle: 来自Jekyll模板编写
---
<div class="box12 div-shadow div-radius">
<div class="bg22"></div>
<div>
<img src="https://i.loli.net/2020/07/10/tW2fu3hFmGZVgJQ.jpg" alt="">
</div>

</div>
<div class="cs1 cs2 mar-zero div-shadow">
{% assign postsCategory = site.posts | group_by_exp:"post", "post.categories"  %}
{% for category in postsCategory %}
<h4 class="post-teaser__month">
<strong>
{% if category.name %} 
- - - - -  {{ category.name }} - - - - - 
{% else %} 
{{ Print }} 
{% endif %}
</strong>
</h4>
<ul class="list-posts">
{% for post in category.items %}
<li class="post-teaser">
<a href="{{ post.url | prepend: site.baseurl }}">
<span class="post-teaser__title">{{ post.title }}</span>
<span class="post-teaser__date">{{ post.date | date: "%d %B %Y" }}</span>
</a>
</li>
{% endfor %}
</ul>
{% endfor %}
</div>