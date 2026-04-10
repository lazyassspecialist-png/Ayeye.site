---
layout: default
title: Home
---

<div class="hero">
  <h1>AI Tools That Actually Build Side Income</h1>
  <p>Real reviews. Real results. No fluff.</p>
</div>

<div class="intro">
  <p>We're building side income streams with AI tools — and documenting everything along the way.</p>
  <p>Every tool on this site gets tested in real workflows. Every review is based on actual use, not just features lists.</p>
  <p>If it doesn't help you make money or save time, it doesn't make the cut.</p>
</div>

<style>
  .hero {
    text-align: center;
    padding: 80px 20px;
    background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
    color: white;
    border-radius: 12px;
    margin-bottom: 40px;
  }
  .hero h1 {
    font-size: 2.5rem;
    margin-bottom: 12px;
    color: #e2e8f0;
  }
  .hero p {
    font-size: 1.2rem;
    color: #94a3b8;
  }
  .intro {
    max-width: 700px;
    margin: 0 auto 40px;
    line-height: 1.8;
    font-size: 1.05rem;
    color: #334155;
  }
  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 24px;
    margin-top: 40px;
  }
  .post-card {
    border: 1px solid #e2e8f0;
    border-radius: 10px;
    padding: 24px;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .post-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 24px rgba(0,0,0,0.08);
  }
  .post-card h3 {
    margin: 0 0 10px;
    font-size: 1.15rem;
  }
  .post-card h3 a {
    color: #1e293b;
    text-decoration: none;
  }
  .post-card h3 a:hover {
    color: #2563eb;
  }
  .post-card .date {
    font-size: 0.8rem;
    color: #64748b;
    margin-bottom: 10px;
  }
  .post-card .excerpt {
    font-size: 0.9rem;
    color: #475569;
    line-height: 1.6;
  }
  .category-badge {
    display: inline-block;
    background: #2563eb;
    color: white;
    font-size: 0.7rem;
    padding: 3px 8px;
    border-radius: 4px;
    margin-bottom: 8px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }
  .category-badge.review { background: #059669; }
  .category-badge.guide { background: #7c3aed; }
  .category-badge.comparison { background: #d97706; }
</style>

<div class="post-grid">
  {% for post in site.posts limit:6 %}
    <div class="post-card">
      {% if post.category == "review" %}
        <span class="category-badge review">Review</span>
      {% elsif post.category == "guide" %}
        <span class="category-badge guide">Guide</span>
      {% elsif post.category == "comparison" %}
        <span class="category-badge comparison">Comparison</span>
      {% else %}
        <span class="category-badge">Article</span>
      {% endif %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="date">{{ post.date | date: "%B %d, %Y" }}</p>
      <p class="excerpt">{{ post.excerpt }}</p>
    </div>
  {% endfor %}
</div>