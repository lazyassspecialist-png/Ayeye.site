---
layout: default
title: Home
---

<!-- Hero -->
<section class="hero">
  <p class="hero-eyebrow">
    <span class="hero-eyebrow-dot"></span>
    Side income with AI — tested in real workflows
  </p>
  <h1>Tools that actually build<br>side income</h1>
  <p class="hero-sub">We test every AI tool before recommending it. No features lists. No fluff. Real results, documented honestly — because our income depends on it.</p>
  <div style="display:flex;gap:10px;flex-wrap:wrap;">
    <a href="/reviews/" class="btn btn-primary">Browse reviews</a>
    <a href="/guides/" class="btn btn-outline">Read guides</a>
  </div>
</section>

<hr class="divider">

<!-- Featured Reviews -->
<section class="posts-section">
  <div class="section-header">
    <h2 class="section-title">Featured</h2>
    <a href="/reviews/" class="section-link">View all →</a>
  </div>
  <div class="post-grid">
    {% for post in site.posts limit:6 %}
    <div class="post-card">
      <div class="post-card-top">
        <span class="post-category">{{ post.category }}</span>
      </div>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="excerpt">{{ post.excerpt }}</p>
      <div class="post-card-footer">
        <span class="post-date">{{ post.date | date: "%b %Y" }}</span>
        <a href="{{ post.url }}" class="read-more">Read →</a>
      </div>
    </div>
    {% endfor %}
  </div>
</section>

<hr class="divider">

<!-- Top Tools -->
<section class="posts-section">
  <div class="section-header">
    <h2 class="section-title">Recommended</h2>
  </div>
  <div class="tools-grid">
    <div class="tool-card">
      <div class="tool-card-top">
        <span class="tool-rating">9/10</span>
        <span class="tool-category">Email</span>
      </div>
      <h3><a href="/reviews/convertkit-review/">ConvertKit</a></h3>
      <p class="excerpt">Best email platform for creators and affiliate marketers. 30% recurring commission on every user you refer — forever.</p>
    </div>
    <div class="tool-card">
      <div class="tool-card-top">
        <span class="tool-rating">8.5/10</span>
        <span class="tool-category">AI Writing</span>
      </div>
      <h3><a href="/reviews/jasper-ai-review/">Jasper AI</a></h3>
      <p class="excerpt">The strongest AI writing tool for affiliate content. Boss Mode + SurferSEO is the combo for publishing at scale without losing quality.</p>
    </div>
    <div class="tool-card">
      <div class="tool-card-top">
        <span class="tool-rating">8/10</span>
        <span class="tool-category">Courses</span>
      </div>
      <h3><a href="/reviews/thinkific-review/">Thinkific</a></h3>
      <p class="excerpt">Create and sell courses without being a developer. Better free plan than Teachable. 30% recurring affiliate commission.</p>
    </div>
  </div>
</section>

<p class="disclosure">Affiliate disclosure: We earn a commission when you purchase through links on this site — at no extra cost to you. We only recommend tools we've tested and believe in.</p>