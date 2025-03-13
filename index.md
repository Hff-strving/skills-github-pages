---
layout: default
title: 我的技术博客
description: 记录学习历程，分享技术心得
---

<link rel="stylesheet" href="{{ site.baseurl }}/assets/css/style.css">

<div class="hero-section">
  <h1>👋 Welcome to FanFan's Blog</h1>
  <p class="subtitle">技术探索 • 学习分享 • 生活感悟</p>
</div>

<div class="featured-posts">
  <h2>📚 最新文章</h2>
  <div class="post-grid">
    {% for post in site.posts limit:3 %}
    <div class="post-card">
      <div class="post-date">{{ post.date | date: "%Y-%m-%d" }}</div>
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
      <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <div class="post-tags">
        {% for tag in post.tags %}
        <span class="tag">{{ tag }}</span>
        {% endfor %}
      </div>
    </div>
    {% endfor %}
  </div>
</div>

<div class="content-sections">
  <div class="section">
    <h2>💡 专题分类</h2>
    <div class="category-list">
      <div class="category-item">
        <h3>🔥 LeetCode 题解</h3>
        <ul>
          {% for post in site.categories.leetcode limit:5 %}
          <li>
            <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
            <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
          </li>
          {% endfor %}
        </ul>
      </div>
      
      <div class="category-item">
        <h3>📝 技术笔记</h3>
        <ul>
          {% for post in site.categories.tech limit:5 %}
          <li>
            <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
            <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
          </li>
          {% endfor %}
        </ul>
      </div>
    </div>
  </div>

  <div class="about-section">
    <h2>🙋‍♂️ 关于我</h2>
    <div class="profile-card">
      <div class="profile-info">
        <h3>Hff-strving</h3>
        <p>热爱编程的学生 | 算法爱好者 | 运动达人</p>
        <ul class="interests">
          <li>💻 编程学习</li>
          <li>🏓 乒乓球</li>
          <li>🏃‍♂️ 跑步</li>
        </ul>
      </div>
      <div class="social-links">
        <a href="https://github.com/hff-strving" target="_blank" class="social-link">
          <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub">
          GitHub
        </a>
        <a href="https://blog.csdn.net/2303_82270449" target="_blank" class="social-link">
          <img src="https://g.csdnimg.cn/static/logo/favicon32.ico" alt="CSDN">
          CSDN
        </a>
      </div>
    </div>
  </div>
</div>

<div class="stats-section">
  <h2>📊 博客统计</h2>
  <div class="stats-grid">
    <div class="stat-card">
      <div class="stat-number">{{ site.posts | size }}</div>
      <div class="stat-label">文章总数</div>
    </div>
    <div class="stat-card">
      <div class="stat-number">{{ site.categories | size }}</div>
      <div class="stat-label">分类数量</div>
    </div>
    <div class="stat-card">
      <div class="stat-number">{{ site.tags | size }}</div>
      <div class="stat-label">标签总数</div>
    </div>
  </div>
</div>
