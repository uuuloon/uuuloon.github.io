---
layout: page
permalink: /resume/
title: resume
nav: true
nav_order: 5
---

<style>
  .post-header, .post-title { display: none !important; }
  .download-link { text-align: center; margin: 15px 0; font-family: monospace; }
  .download-link a { text-decoration: none; font-size: 1.1rem; }
  .download-link a:hover { text-decoration: underline; }
  .resume-container { 
    border: 1px solid #444; 
    border-radius: 8px; 
    overflow: hidden; 
    background: white;
    color-scheme: light;
    height: 85vh;
    min-height: 500px;
    margin: 20px 0;
    width: 100%;
  }
  .resume-container iframe {
    width: 100%;
    height: 100%;
    border: none;
  }
</style>

<div class="download-link">
  <a href="{{ '/assets/pdf/Resume.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer">
    Download Resume
  </a>
</div>

<div class="resume-container">
  <iframe src="{{ '/assets/pdf/Resume.pdf' | relative_url }}#toolbar=0&view=FitH" title="Resume Preview"></iframe>
</div>
