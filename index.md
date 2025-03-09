---
layout: default
title: 我的个人博客
description: 欢迎来到我的个人博客，这里分享我的技术学习和生活感悟。
---

<link rel="stylesheet" href="{{ site.baseurl }}/assets/css/style.css">

# 欢迎来到我的博客！ 👋

你好！这是我的个人博客，使用 GitHub Pages 和 Jekyll 搭建。我会在这里分享我的技术学习、项目经验和生活感悟。

<div class="container">
    <!-- LeetCode 题解 -->
    <div class="left-column">
        <h2>📌 LeetCode 题解</h2>
        <ul>
            {% for post in site.categories.leetcode %}
            <li>
                <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}
            </li>
            {% endfor %}
        </ul>
    </div>

    <!-- 日常分享 -->
    <div class="right-column">
        <h2>🌟 日常分享</h2>
        <ul>
            {% for post in site.categories.daily %}
            <li>
                <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}
            </li>
            {% endfor %}
        </ul>
    </div>
</div>

## 🙋 关于我

- **姓名**: Hff-strving
- **职业**: 学生
- **兴趣**: CSDN, LeetCode, 乒乓球, 跑步

---

## 🔗 友情链接

- [GitHub](https://github.com/hff-strving)
- [CSDN](https://blog.csdn.net/2303_82270449?spm=1010.2135.3001.5421)
