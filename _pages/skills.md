---
permalink: /skills/
title: "Skills & Expertise"
author_profile: false
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/skills-header.jpg
excerpt: "Technical Skills & Proficiencies"
---

<style>
  .skills-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 25px;
    margin: 30px 0;
  }

  .skill-box {
    background: linear-gradient(135deg, #1e3a8a 0%, #7c3aed 100%);
    padding: 30px;
    border-radius: 12px;
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
    border-top: 4px solid #4ade80;
    transition: all 0.3s ease;
  }

  .skill-box:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 40px rgba(74, 222, 128, 0.3);
    border-top-color: #60a5fa;
  }

  .skill-box h3 {
    color: #60a5fa;
    margin-bottom: 20px;
    font-size: 20px;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .skill-list {
    list-style: none;
    padding: 0;
  }

  .skill-list li {
    color: #e2e8f0;
    padding: 10px 0;
    border-bottom: 1px solid rgba(96, 165, 250, 0.2);
    display: flex;
    align-items: center;
  }

  .skill-list li:last-child {
    border-bottom: none;
  }

  .skill-list li:before {
    content: "▶";
    color: #4ade80;
    font-weight: bold;
    margin-right: 10px;
  }

  .progress-bar {
    background: rgba(255, 255, 255, 0.1);
    height: 8px;
    border-radius: 4px;
    margin-top: 10px;
    overflow: hidden;
  }

  .progress-fill {
    height: 100%;
    background: linear-gradient(90deg, #4ade80 0%, #60a5fa 100%);
    border-radius: 4px;
    animation: fillProgress 1.5s ease-out forwards;
  }

  @keyframes fillProgress {
    from {
      width: 0%;
    }
    to {
      width: var(--progress, 80%);
    }
  }

  .certification-badge {
    display: inline-block;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 12px 20px;
    border-radius: 20px;
    margin: 8px;
    font-weight: 500;
    box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);
    transition: all 0.3s ease;
  }

  .certification-badge:hover {
    transform: scale(1.05);
    box-shadow: 0 6px 20px rgba(102, 126, 234, 0.5);
  }
</style>

## 🎯 Technical Skills & Expertise

My skill set spans across cybersecurity, programming, and cloud technologies. Here's a comprehensive breakdown:

---

## 🔐 Cybersecurity Skills

<div class="skills-container">

<div class="skill-box">
<h3>🕵️ Penetration Testing</h3>
<ul class="skill-list">
<li>Network Reconnaissance</li>
<li>Vulnerability Scanning</li>
<li>Exploitation Techniques</li>
<li>Post-Exploitation</li>
<li>Report Generation</li>
</ul>
</div>

<div class="skill-box">
<h3>🔍 Network Security</h3>
<ul class="skill-list">
<li>Network Protocols</li>
<li>Packet Analysis</li>
<li>IDS/IPS Configuration</li>
<li>Firewall Management</li>
<li>DNS/DHCP Security</li>
</ul>
</div>

<div class="skill-box">
<h3>🛡️ Web Security</h3>
<ul class="skill-list">
<li>OWASP Top 10</li>
<li>SQL Injection Testing</li>
<li>XSS Detection</li>
<li>CSRF Mitigation</li>
<li>API Security</li>
</ul>
</div>

<div class="skill-box">
<h3>📋 Compliance & Risk</h3>
<ul class="skill-list">
<li>Risk Assessment</li>
<li>Security Auditing</li>
<li>Vulnerability Management</li>
<li>Incident Response</li>
<li>Security Policies</li>
</ul>
</div>

<div class="skill-box">
<h3>🔬 Malware Analysis</h3>
<ul class="skill-list">
<li>Static Analysis</li>
<li>Dynamic Analysis</li>
<li>Reverse Engineering</li>
<li>Behavior Analysis</li>
<li>Threat Intelligence</li>
</ul>
</div>

<div class="skill-box">
<h3>☁️ Cloud Security</h3>
<ul class="skill-list">
<li>AWS Security</li>
<li>Cloud Architecture</li>
<li>Identity Management</li>
<li>Data Protection</li>
<li>Compliance (SOC 2)</li>
</ul>
</div>

</div>

---

## 💻 Programming Languages

<div class="skills-container">

<div class="skill-box">
<h3>🐍 Python</h3>
<p style="color: #e2e8f0; margin-bottom: 10px;"><strong>Proficiency: Advanced</strong></p>
<div class="progress-bar">
<div class="progress-fill" style="--progress: 85%;"></div>
</div>
<p style="color: #cbd5e1; margin-top: 10px; font-size: 14px;">Socket programming, threading, automation scripts, security tools development</p>
</div>

<div class="skill-box">
<h3>C Language</h3>
<p style="color: #e2e8f0; margin-bottom: 10px;"><strong>Proficiency: Intermediate</strong></p>
<div class="progress-bar">
<div class="progress-fill" style="--progress: 70%;"></div>
</div>
<p style="color: #cbd5e1; margin-top: 10px; font-size: 14px;">Systems programming, memory management, data structures</p>
</div>

<div class="skill-box">
<h3>Java</h3>
<p style="color: #e2e8f0; margin-bottom: 10px;"><strong>Proficiency: Intermediate</strong></p>
<div class="progress-bar">
<div class="progress-fill" style="--progress: 70%;"></div>
</div>
<p style="color: #cbd5e1; margin-top: 10px; font-size: 14px;">OOP concepts, application development, security frameworks</p>
</div>

<div class="skill-box">
<h3>Web Technologies</h3>
<p style="color: #e2e8f0; margin-bottom: 10px;"><strong>Proficiency: Intermediate</strong></p>
<div class="progress-bar">
<div class="progress-fill" style="--progress: 65%;"></div>
</div>
<p style="color: #cbd5e1; margin-top: 10px; font-size: 14px;">HTML/CSS/JavaScript, Web frameworks, Frontend security</p>
</div>

<div class="skill-box">
<h3>Bash/Shell</h3>
<p style="color: #e2e8f0; margin-bottom: 10px;"><strong>Proficiency: Advanced</strong></p>
<div class="progress-bar">
<div class="progress-fill" style="--progress: 80%;"></div>
</div>
<p style="color: #cbd5e1; margin-top: 10px; font-size: 14px;">System administration, automation, scripting for security tasks</p>
</div>

<div class="skill-box">
<h3>SQL</h3>
<p style="color: #e2e8f0; margin-bottom: 10px;"><strong>Proficiency: Intermediate</strong></p>
<div class="progress-bar">
<div class="progress-fill" style="--progress: 70%;"></div>
</div>
<p style="color: #cbd5e1; margin-top: 10px; font-size: 14px;">Database queries, injection testing, data analysis</p>
</div>

</div>

---

## 🛠️ Tools & Platforms

### Security Tools
<div style="margin: 20px 0;">
<span class="certification-badge">🎯 Nmap</span>
<span class="certification-badge">🎯 Burp Suite</span>
<span class="certification-badge">🎯 Wireshark</span>
<span class="certification-badge">🎯 Metasploit</span>
<span class="certification-badge">🎯 Kali Linux</span>
<span class="certification-badge">🎯 OWASP ZAP</span>
<span class="certification-badge">🎯 Snort/Suricata</span>
<span class="certification-badge">🎯 Hashcat</span>
</div>

### Learning Platforms
<div style="margin: 20px 0;">
<span class="certification-badge">📚 TryHackMe</span>
<span class="certification-badge">📚 Hack The Box</span>
<span class="certification-badge">📚 OWASP WebGoat</span>
<span class="certification-badge">📚 Coding Ninjas</span>
<span class="certification-badge">📚 HackerRank</span>
</div>

### Development & DevOps
<div style="margin: 20px 0;">
<span class="certification-badge">⚙️ Git/GitHub</span>
<span class="certification-badge">⚙️ Docker</span>
<span class="certification-badge">⚙️ Linux</span>
<span class="certification-badge">⚙️ AWS</span>
<span class="certification-badge">⚙️ VS Code</span>
</div>

---

## 📈 Skill Development Timeline

| Skill Category | Current Level | Target Level | Timeline |
|---|---|---|---|
| Penetration Testing | Intermediate | Advanced | 6 months |
| Network Security | Intermediate | Expert | 8 months |
| Python Development | Advanced | Expert | 3 months |
| Malware Analysis | Beginner | Intermediate | 6 months |
| Cloud Security | Intermediate | Advanced | 4 months |
| CEH Certification | In Progress | Completed | 2 months |

---

## 🎓 Certifications & Badges

<div style="margin: 30px 0;">
<span class="certification-badge">🏆 CEH v13 (In Progress)</span>
<span class="certification-badge">🏆 Oracle Cloud Infrastructure</span>
<span class="certification-badge">🏆 Dell GenAI Foundations</span>
<span class="certification-badge">🏆 Deloitte Cyber Security</span>
<span class="certification-badge">🏆 Data Analytics (Coding Ninjas)</span>
<span class="certification-badge">🏆 Ethical Hacking (NSDC)</span>
<span class="certification-badge">🏆 Python Programming</span>
</div>

---

## 🎯 Continuous Learning

I'm committed to staying updated with the latest cybersecurity trends and technologies through:
- Regular practice on CTF platforms
- Reading security research papers
- Following industry experts and communities
- Attending webinars and security conferences
- Building practical projects
- Contributing to open-source security projects

**Current Focus:** CEH v13 Certification & Advanced Penetration Testing

[← Back to Home](/) | [View Projects](/projects/) | [Read Blog](/blog/)

