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
excerpt: "🎯 BTech Cybersecurity Student | 🔐 Ethical Hacker | 🐍 Python Developer | Building Practical Security Solutions"
---

<style>
  /* Better spacing for congested sections */
  .hero-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    padding: 50px 30px;
    border-radius: 10px;
    margin: 50px 0;
    box-shadow: 0 8px 32px rgba(102, 126, 234, 0.3);
    animation: slideIn 0.8s ease-out;
  }

  /* FIX: Add breathing room between stat cards */
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 30px;
    margin: 60px 0;
    padding: 0 20px;
  }

  .stat-card {
    background: linear-gradient(135deg, #1e3a8a 0%, #7c3aed 100%);
    padding: 35px;
    border-radius: 12px;
    text-align: center;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    min-height: 160px;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .stat-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 35px rgba(124, 58, 237, 0.4);
  }

  .stat-number {
    font-size: 36px;
    font-weight: bold;
    color: #4ade80;
    animation: countUp 2s ease-out forwards;
    margin-bottom: 10px;
  }

  .stat-label {
    color: #cbd5e1;
    margin-top: 0;
    font-size: 15px;
    line-height: 1.4;
  }

  /* FIX: Add proper spacing between sections */
  .section-spacer {
    height: 40px;
  }

  .featured-projects {
    margin: 80px 0;
    padding: 0 20px;
  }

  .project-card {
    background: linear-gradient(135deg, rgba(30, 58, 138, 0.8) 0%, rgba(124, 58, 237, 0.8) 100%);
    padding: 40px;
    border-radius: 12px;
    border-left: 5px solid #4ade80;
    margin: 30px 0;
    transition: all 0.3s ease;
    backdrop-filter: blur(10px);
  }

  .project-card:hover {
    transform: translateX(8px);
    box-shadow: 0 10px 40px rgba(74, 222, 128, 0.25);
    border-left-color: #60a5fa;
  }

  .project-title {
    font-size: 24px;
    font-weight: bold;
    color: #60a5fa;
    margin-bottom: 15px;
    margin-top: 0;
  }

  .project-desc {
    color: #e2e8f0;
    line-height: 1.8;
    font-size: 16px;
    margin-bottom: 20px;
  }

  .cta-buttons {
    display: flex;
    gap: 15px;
    margin-top: 40px;
    flex-wrap: wrap;
  }

  .btn {
    padding: 12px 25px !important;
    font-size: 15px !important;
  }

  @keyframes slideIn {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes countUp {
    from {
      opacity: 0;
      transform: scale(0.8);
    }
    to {
      opacity: 1;
      transform: scale(1);
    }
  }

  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .hero-section {
      padding: 35px 20px;
      margin: 30px 10px;
    }
    
    .stats-grid {
      gap: 20px;
      margin: 40px 0;
      padding: 0 10px;
    }

    .stat-card {
      padding: 25px;
      min-height: 140px;
    }

    .stat-number {
      font-size: 28px;
    }

    .project-card {
      padding: 25px;
      margin: 20px 0;
    }

    .cta-buttons {
      flex-direction: column;
    }
  }
</style>

## 🎯 Welcome to My Cybersecurity Portfolio

I'm **Sachin Singh Tanwar**, a passionate cybersecurity student and ethical hacker building practical security solutions and learning advanced hacking techniques.

<div class="section-spacer"></div>

---

## 📊 Quick Overview

<div class="stats-grid">
  <div class="stat-card">
    <div class="stat-number">7+</div>
    <div class="stat-label">Certifications Earned</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">1+</div>
    <div class="stat-label">Projects Built</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">∞</div>
    <div class="stat-label">Learning Journey</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">100%</div>
    <div class="stat-label">Commitment</div>
  </div>
</div>

<div class="section-spacer"></div>

---

## 🚀 Featured Project

<div class="featured-projects">
  <div class="project-card">
    <h3 class="project-title">🔍 Port Scanner & Reconnaissance Tool</h3>
    <p class="project-desc">
      A professional Python-based network scanner featuring multi-threading, banner grabbing, and advanced reconnaissance capabilities. This project demonstrates core CEH footprinting and reconnaissance techniques.
    </p>
    <div class="cta-buttons">
      <a href="/projects/" class="btn btn--info">📂 Explore Projects</a>
      <a href="https://github.com/SachinRajput-SSR/port-scanner-project" class="btn btn--success">🐙 View on GitHub</a>
    </div>
  </div>
</div>

<div class="section-spacer"></div>

---

## 🎓 My Journey: Zero to Hero

