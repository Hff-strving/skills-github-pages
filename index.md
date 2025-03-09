---
layout: default
title: 我的个人博客
description: 欢迎来到我的个人博客，这里分享我的技术学习和生活感悟。
---

<link rel="stylesheet" href="{{ site.baseurl }}/assets/css/style.css">

<div class="header">
  <h1>欢迎来到我的博客！ 👋</h1>
  <p>你好！这是我的个人博客，使用 GitHub Pages 和 Jekyll 搭建。我会在这里分享我的技术学习、项目经验和生活感悟。</p>
</div>

---

<div class="categories">
  <h2>📝 博客分类</h2>

  <div class="category">
    <h3>📌 LeetCode 题解</h3>
    <ul>
      {% for post in site.categories.leetcode %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}</li>
      {% endfor %}
    </ul>
  </div>

  <div class="category">
    <h3>🌟 日常分享</h3>
    <ul>
      {% for post in site.categories.daily %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}</li>
      {% endfor %}
    </ul>
  </div>
</div>

---

<div class="about-me">
  <h2>🙋 关于我</h2>
  <ul>
    <li><strong>姓名</strong>: Hff-strving</li>
    <li><strong>职业</strong>: 学生</li>
    <li><strong>兴趣</strong>: CSDN, LeetCode, 乒乓球, 跑步</li>
  </ul>
</div>

---

<div class="links">
  <h2>🔗 友情链接</h2>
  <ul>
    <li><a href="https://github.com/hff-strving">GitHub</a></li>
    <li><a href="https://blog.csdn.net/2303_82270449?spm=1010.2135.3001.5421">CSDN</a></li>
  </ul>
</div>
