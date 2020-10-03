---
layout: page3
title: 个人博客
subtitle: 来自Jekyll模板编写
---
<div>
<div class="box12 div-shadow div-radius">
<div class="bg22"></div>
<div class="div-ai-center div-fd-column  div-stWidth">
<div class="mar-zero">
<img src="https://i.loli.net/2020/07/10/tW2fu3hFmGZVgJQ.jpg" alt="">
</div>
<p>GikoMax</p>
<p>一条没技术的咸鱼</p>
</div>

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
<div>
<div class="box1231 div-shadow div-radius">
 <h4 class="as1">公告日志</h4>
 <div>2020-10-3个人简介页面更新 添加头像hover效果 做出技能点进度条
 <br>2020-10-3更新 主页大更新<br>留言区暂时未开放更多功能请敬请期待
 <br>2020-9-20 完全修改index页面 修改主页效果为当前模样

 </div>
</div>
</div>
