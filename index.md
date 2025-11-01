---
layout: home
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
  overlay_image: /assets/images/cyber-header.jpg
  actions:
    - label: "🔍 View Projects"
      url: "/projects/"
    - label: "📖 Learn More"
      url: "/about/"
excerpt: "🎯 BTech Cybersecurity Student | 🔐 Certified Ethical Hacker | 🐍 Python Developer | Building Practical Security Solutions"
---

<style>
  .hero-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    padding: 40px 20px;
    border-radius: 10px;
    margin: 30px 0;
    box-shadow: 0 8px 32px rgba(102, 126, 234, 0.3);
    animation: slideIn 0.8s ease-out;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin: 30px 0;
  }

  .stat-card {
    background: linear-gradient(135deg, #1e3a8a 0%, #7c3aed 100%);
    padding: 25px;
    border-radius: 12px;
    text-align: center;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .stat-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(124, 58, 237, 0.4);
  }

  .stat-number {
    font-size: 32px;
    font-weight: bold;
    color: #4ade80;
    animation: countUp 2s ease-out forwards;
  }

  .stat-label {
    color: #cbd5e1;
    margin-top: 8px;
    font-size: 14px;
  }

  @keyframes slideIn {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes countUp {
    from {
      opacity: 0;
      transform: scale(0.5);
    }
    to {
      opacity: 1;
      transform: scale(1);
    }
  }

  .featured-projects {
    margin: 50px 0;
  }

  .project-card {
    background: linear-gradient(135deg, rgba(30, 58, 138, 0.8) 0%, rgba(124, 58, 237, 0.8) 100%);
    padding: 30px;
    border-radius: 12px;
    border-left: 4px solid #4ade80;
    margin: 20px 0;
    transition: all 0.3s ease;
    backdrop-filter: blur(10px);
  }

  .project-card:hover {
    transform: translateX(5px);
    box-shadow: 0 8px 32px rgba(74, 222, 128, 0.2);
    border-left-color: #60a5fa;
  }

  .project-title {
    font-size: 20px;
    font-weight: bold;
    color: #60a5fa;
    margin-bottom: 10px;
  }

  .project-desc {
    color: #e2e8f0;
    line-height: 1.6;
  }
</style>

## 🎯 Welcome to My Cybersecurity Portfolio

I'm **Sachin Singh Tanwar**, a passionate cybersecurity student and Certified Ethical Hacker dedicated to building secure systems and protecting digital infrastructure. This is my journey from **zero to hero** in cybersecurity through practical projects, certifications, and continuous learning.

---

## 📊 Quick Overview

<div class="stats-grid">
  <div class="stat-card">
    <div class="stat-number">7+</div>
    <div class="stat-label">Certifications</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">1+</div>
    <div class="stat-label">Projects</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">∞</div>
    <div class="stat-label">Learning Path</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">100%</div>
    <div class="stat-label">Dedication</div>
  </div>
</div>

---

## 🚀 Featured Project

<div class="featured-projects">
  <div class="project-card">
    <div class="project-title">🔍 Port Scanner & Reconnaissance Tool</div>
    <div class="project-desc">
      A professional Python-based network scanner with multi-threading, banner grabbing, and advanced reconnaissance capabilities. Demonstrates core CEH footprinting and reconnaissance techniques.
    </div>
    <br>
    <a href="/projects/" class="btn btn--info">Explore Projects →</a>
  </div>
</div>

---

## 🎓 Learning Path: Beginner → Advanced

Phase 1: Foundations ✅ → Phase 2: Intermediate 🔄 → Phase 3: Advanced 📈 → Phase 4: Expert 🎯

- **Beginner:** Port scanning, basic Python, networking fundamentals
- **Intermediate:** Automation, monitoring, incident response
- **Advanced:** AI/ML in cybersecurity, deception technology, IoT security

---

## 🔗 Connect With Me

<div style="margin-top: 30px; text-align: center;">
  <a href="https://www.linkedin.com/in/sachin-singh-tanwar-5582582b4/" class="btn btn--info btn--large" style="margin: 10px;">LinkedIn</a>
  <a href="https://github.com/SachinRajput-SSR" class="btn btn--info btn--large" style="margin: 10px;">GitHub</a>
  <a href="mailto:your-email@example.com" class="btn btn--info btn--large" style="margin: 10px;">Email</a>
</div>

---

**Latest Update:** {{ site.time | date: "%B %d, %Y" }}

