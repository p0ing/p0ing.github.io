---
layout: default
title: 주제2 전체 글 보기
permalink: /topic2/
---

# 📁 주제2 전체 목록
이곳은 '주제2'에 해당하는 모든 글을 모아놓은 공간입니다.

<ul>
<!-- 여기는 limit:5 가 없으므로 모든 글이 출력됩니다 -->
{% for post in site.categories["주제2"] %}
  <li>
    <span>{{ post.date | date: "%Y-%m-%d" }}</span> &raquo; 
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>