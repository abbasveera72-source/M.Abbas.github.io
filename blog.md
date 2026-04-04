---
layout: page
title: Blog
permalink: /blog/
---

<div style="text-align: center; max-width: 800px; margin: 20px auto;">
  <h1 style="color: #1a1a1a; border: none;">Technical Insights</h1>
  <p style="color: #666;">A collection of my research, lab reports, and personal experiences.</p>
  <hr style="width: 60px; margin: 20px auto; border: 0; border-top: 3px solid #007bff;">
</div>

<div style="max-width: 800px; margin: 0 auto;">
  {% for post in site.posts %}
  <div style="padding: 25px; margin-bottom: 20px; border: 1px solid #e1e4e8; border-radius: 10px; background: white; transition: 0.3s; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
    <span style="color: #007bff; font-weight: bold; font-size: 0.85rem;">{{ post.date | date: "%B %d, %Y" }}</span>
    <h3 style="margin: 10px 0;">
      <a href="{{ post.url | relative_url }}" style="color: #1a1a1a; text-decoration: none; border-bottom: 2px solid transparent;">{{ post.title }}</a>
    </h3>
    <p style="color: #555; font-size: 0.95rem; line-height: 1.5;">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    <a href="{{ post.url | relative_url }}" style="color: #007bff; font-weight: bold; text-decoration: none; font-size: 0.9rem;">Read Full Post →</a>
  </div>
  {% endfor %}
</div>
