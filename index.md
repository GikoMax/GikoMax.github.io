---
layout: page
title: 别来无恙！
subtitle: 这里是GikoMax的个人技术博客
sitemap:
  priority: 0.9
---


<img src="{{ '/assets/img/logo.jpg' | prepend: site.baseurl }}" id="about-img">
<div class="blob animated">
  <div class="eyes">
    <div class="eye left-eye"></div>
    <div class="eye right-eye"></div>
  </div>
  <div class="mouth"></div>
</div>

<script>
/* 
 How can geometry
 bear affection?
 It's the purest love:
 projection.
*/

const animationType = 'headShake'
const blob = document.querySelectorAll('.blob')[0];
const body = document.getElementsByTagName('body')[0];

blob.addEventListener('mouseenter', () => {
  blob.classList.add(animationType);
});

blob.addEventListener('mouseleave', () => {
  blob.classList.remove(animationType);
});

body.addEventListener('mousemove', (e) => {
  if (e.clientY < blob.offsetHeight) {
    blob.classList.add('look-up');
  } else {
    blob.classList.remove('look-up');
  }
  
  if (e.clientY > (blob.offsetHeight + 150)) {
    blob.classList.add('look-down');
  } else {
    blob.classList.remove('look-down');
  }


  if (e.clientX < (blob.offsetLeft)) {
    blob.classList.add('look-left');
  } else {
    blob.classList.remove('look-left');
  }  

  if (e.clientX > (blob.offsetLeft + 235)) {
    blob.classList.add('look-right');
  } else {
    blob.classList.remove('look-right');
  }   
});
</script>
<div style="text-align:center;">
</div>
<div id="describe-text">
	<p>A simple, minimal Jekyll theme for a personal web page and blog, focusing on white space and readability</p>
	<p>Fork and use the theme from the <strong> <a href="https://github.com/knhash/Pudhina"> repository</a> </strong></p>
</div>