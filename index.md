---
layout: default
title: Home
---

<!-- Hero -->
<section class="hero">
  <span class="hero-eyebrow">
    <span class="hero-eyebrow-dot"></span>
    Side income with AI — tested and documented
  </span>
  <h1>AI Tools That Actually Build <span class="accent-word">Side Income</span></h1>
  <p class="hero-sub">Real reviews. Real results. We test every tool in actual workflows — no features lists, no fluff. If it doesn't help you make money or save time, it doesn't make the cut.</p>
  <div class="hero-actions">
    <a href="/reviews/" class="btn btn-primary">Browse Reviews</a>
    <a href="/guides/" class="btn btn-secondary">Read Guides</a>
  </div>
</section>

<!-- Intro -->
<section class="intro">
  <div class="intro-grid">
    <div class="intro-item">
      <h3>📊 Our Approach</h3>
      <p>We're building side income with AI tools right now. Every review on this site comes from 2+ weeks of real use — not AI-generated summaries or spec sheet rewrites.</p>
    </div>
    <div class="intro-item">
      <h3>💰 Our Incentive</h3>
      <p>We use affiliate links because they align our success with yours. When a tool works, we recommend it. When it doesn't, we tell you. Simple as that.</p>
    </div>
  </div>
</section>

<!-- Latest Articles -->
<section class="posts-section">
  <div class="section-header">
    <h2 class="section-title">Latest Articles</h2>
    <a href="/reviews/" class="section-link">View all →</a>
  </div>
  <div class="post-grid">
    {% for post in site.posts limit:6 %}
    <div class="post-card">
      <div class="post-card-top">
        {% if post.category == "review" %}
          <span class="category-badge review">Review</span>
        {% elsif post.category == "guide" %}
          <span class="category-badge guide">Guide</span>
        {% elsif post.category == "comparison" %}
          <span class="category-badge comparison">Comparison</span>
        {% else %}
          <span class="category-badge article">Article</span>
        {% endif %}
        <span class="post-meta">{{ post.date | date: "%B %Y" }}</span>
      </div>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="excerpt">{{ post.excerpt }}</p>
      <div class="post-card-footer">
        <a href="{{ post.url }}" class="read-more">Read more →</a>
      </div>
    </div>
    {% endfor %}
  </div>
</section>

<!-- Top Tools Section -->
<section class="posts-section">
  <div class="section-header">
    <h2 class="section-title">Top Tools We Recommend</h2>
  </div>
  <div class="post-grid">
    <div class="post-card" style="border-left: 3px solid #059669;">
      <div class="post-card-top">
        <span class="category-badge review">9/10</span>
        <span class="post-meta">Email Marketing</span>
      </div>
      <h3><a href="/reviews/convertkit-review/">ConvertKit</a></h3>
      <p class="excerpt">Best email platform for creators and affiliate marketers. 30% recurring affiliate commission. Clean interface, powerful automation.</p>
      <div class="post-card-footer">
        <a href="/reviews/convertkit-review/" class="read-more">Read review →</a>
      </div>
    </div>
    <div class="post-card" style="border-left: 3px solid #2563EB;">
      <div class="post-card-top">
        <span class="category-badge review">8.5/10</span>
        <span class="post-meta">AI Writing</span>
      </div>
      <h3><a href="/reviews/jasper-ai-review/">Jasper AI</a></h3>
      <p class="excerpt">The strongest AI writing tool for affiliate content. Boss Mode + SurferSEO integration is the killer combo for publishing at scale.</p>
      <div class="post-card-footer">
        <a href="/reviews/jasper-ai-review/" class="read-more">Read review →</a>
      </div>
    </div>
    <div class="post-card" style="border-left: 3px solid #7C3AED;">
      <div class="post-card-top">
        <span class="category-badge review">8/10</span>
        <span class="post-meta">Course Platform</span>
      </div>
      <h3><a href="/reviews/thinkific-review/">Thinkific</a></h3>
      <p class="excerpt">Create and sell courses without being a tech person. 30% recurring affiliate commissions. Better free plan than Teachable.</p>
      <div class="post-card-footer">
        <a href="/reviews/thinkific-review/" class="read-more">Read review →</a>
      </div>
    </div>
  </div>
</section>

<!-- Affiliate Disclosure -->
<div class="disclosure" style="max-width: 760px; margin: 0 auto 40px;">
  <strong>Affiliate Disclosure:</strong> This site contains affiliate links. If you make a purchase through one of our links, we earn a small commission at no extra cost to you. We only recommend tools we've personally tested and genuinely believe in.
</div>