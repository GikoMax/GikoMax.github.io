---
layout: page1
sitemap:
  priority: 0.9
---
<div style="border: 5px solid white;border-radius:50%;margin-right: auto; margin-left: auto"><img src="https://i.loli.net/2020/07/10/tW2fu3hFmGZVgJQ.jpg" alt="about me" class="blog-entry-img" style="height:200px;border-radius:50%;"></div> 

<div style="margin-right: auto; margin-left: auto"><h1>GikoMax</h1></div>
<div class="centericon">
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
</div>
<div id="describe-text">
	<p>一个简单的，最小的Jekyll主题为个人网页和博客，欢迎大家观看</p>
	<p>想和我联系？当然没问题点这！ <strong> <a href="tencent://message/?uin=824356334&Site=Sambow&Menu=yes"> 联系我的QQ</a> </strong></p>
</div>