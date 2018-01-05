---
layout: home
---

<div class="index-content blog">
    <style>
    .entry {
        box-shadow: none;
    }
    .entry ul li {
        list-style-type: none;
    }
    .index-content .cate-bar{
        margin-bottom:50px;
    }
    </style>

    <div class="section">
        <ul class="artical-cate">
            <li ><a href="/"><span>Blog</span></a></li>
            <!--li style="text-align:center"><a href="/dump"><span>Dump</span></a></li-->
            <li style="text-align:right"><a href="/about"><span>About</span></a></li>
            <li class="on" style="text-align:right"><a href="/archive"><span>Archive</span></a></li>
        </ul>

        <div class="cate-bar"><span id="cateBar"></span></div>
        <div class="entry">
            <ul>
            {% for post in site.posts %}
            	<li><a href='{{ post.url }}' logo='' class='title'> {{ post.date|date_to_string }} - {{ post.title }}</a></li>
            {% endfor %}
            </ul>
    <div class="aside">
    </div>
</div>
