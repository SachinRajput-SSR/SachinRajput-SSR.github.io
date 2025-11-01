---
permalink: /blog/
title: "Blog"
layout: home
author_profile: false
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/blog-header.jpg
excerpt: "Cybersecurity Articles, Tutorials & Technical Write-ups"
paginate: true
---

<style>
  .blog-intro {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    padding: 30px;
    border-radius: 12px;
    margin: 30px 0;
    box-shadow: 0 8px 32px rgba(102, 126, 234, 0.3);
  }

  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 25px;
    margin: 30px 0;
  }

  .post-card {
    background: linear-gradient(135deg, #1e3a8a 0%, #7c3aed 100%);
    border: 1px solid rgba(96, 165, 250, 0.3);
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
    transition: all 0.3s ease;
  }

  .post-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 15px 50px rgba(74, 222, 128, 0.3);
    border-color: #4ade80;
  }

  .post-header {
    padding: 20px;
    border-bottom: 2px solid #4ade80;
  }

  .post-title {
    font-size: 18px;
    font-weight: bold;
    color: #60a5fa;
    margin: 0;
  }

  .post-meta {
    color: #cbd5e1;
    font-size: 12px;
    margin-top: 8px;
  }

  .post-body {
    padding: 20px;
  }

  .post-excerpt {
    color: #e2e8f0;
    line-height: 1.6;
    margin-bottom: 15px;
  }

  .post-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .tag-badge {
    background: rgba(96, 165, 250, 0.2);
    color: #60a5fa;
    padding: 4px 10px;
    border-radius: 12px;
    font-size: 12px;
  }

  .read-more {
    color: #4ade80;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    display: inline-block;
    margin-top: 15px;
  }

  .read-more:hover {
    color: #60a5fa;
  }
</style>

## 📚 Cybersecurity Blog & Technical Articles

<div class="blog-intro">
<h2 style="margin: 0; color: white;">Welcome to My Cybersecurity Blog</h2>
<p style="color: #e2e8f0; margin: 10px 0 0 0;">
Deep dives into cybersecurity concepts, project walkthroughs, tutorials, and lessons learned on my journey from zero to hero. Subscribe and stay updated!
</p>
</div>

---

## Latest Articles

{% for post in site.posts %}

<div class="post-card">
<div class="post-header">
<h3 class="post-title">{{ post.title }}</h3>
<div class="post-meta">
📅 {{ post.date | date: "%B %d, %Y" }} | ⏱️ {% include read-time.html %}
</div>
</div>
<div class="post-body">
<p class="post-excerpt">{{ post.excerpt }}</p>
<div class="post-tags">
{% for tag in post.tags %}
<span class="tag-badge">{{ tag }}</span>
{% endfor %}
</div>
<a href="{{ post.url }}" class="read-more">Read Article →</a>
</div>
</div>

{% endfor %}

---

## 📖 Coming Soon

- 🌐 Personal Website Security Audit - OWASP Top 10 Deep Dive
- 🔐 Secure Password Manager - Cryptography Explained
- 🤖 AI-Powered IDS - Machine Learning in Cybersecurity
- 🍯 Honeypot Deployment - Deception Technology Guide
- 📊 Incident Response - Real-World Case Studies

---

[← Back to Home](/) | [View Projects](/projects/) | [About Me](/about/)

