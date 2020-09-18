---
layout: page1
sitemap:
  priority: 0.9
---
<div style="height:200px;width:200px;border-radius:50%;border: 5px solid white;margin-right: auto; margin-left: auto"><img src="https://i.loli.net/2020/07/10/tW2fu3hFmGZVgJQ.jpg" alt="about me" class="blog-entry-img" style="height:200px;border-radius:50%;margin-right: auto; margin-left: auto"></div> 

<div style="width: 135px;height:100px;margin-right: auto; margin-left: auto"><h1>GikoMax</h1></div>
<div style="border-top: 1px solid #586672;width:20%;height: 1px;margin-right: auto;margin-left: auto; "></div>
<div style="text-align: center;font-size: 40px;margin: 20px">别来无恙!欢迎访问GikoMax的个人博客</div>

 <div style="border-bottom: 2px solid #586672;width:25%;height: 1px;margin-right: auto;margin-left: auto; "></div>
 <div class="midden_1" style="width: 450px;height: 50px;margin: 20px auto 20px auto"><ul class="menu">
      <li><a href="{{ '/resume' | prepend: site.baseurl }}" style="border-radius: 25px;padding:5px;">关于我</a></li>
      <li><a href="{{ '/blog' | prepend: site.baseurl }}" style="border-radius: 25px;padding:5px;">小博客</a></li>
      <li><a href="{{ '/message' | prepend: site.baseurl }}" style="border-radius: 25px;padding:5px;">留言板</a></li>
      </ul>
      </div>
<div class="ii">
<a href="https://github.com/GikoMax/GikoMax.github.io"><i class="fa fa-github" style="font-size:36px"></i></a>
<a href="tencent://message/?uin=824356334&Site=Sambow&Menu=yes"><i class="fa fa-qq" style="font-size:36px"></i></a>
<a href=""><i class="fa fa-weixin" style="font-size:36px"></i></a>
<a href="https://weibo.com/u/6100962481"><i class="fa fa-weibo" style="font-size:36px"></i></a>

</div>
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
<audio src="./MP3/bgm.mp3" autoplay loop controls></audio>
<div id="describe-text">
	<p>一个简单的，最小的Jekyll主题为个人网页和博客，欢迎大家观看</p>
	<p>想和我联系？当然没问题点这！ <strong> <a href="tencent://message/?uin=824356334&Site=Sambow&Menu=yes"> 联系我的QQ</a> </strong></p>
</div>
