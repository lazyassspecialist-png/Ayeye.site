# ayeye.site

AI tools that actually help you build side income — reviewed, tested, recommended.

## 🚀 Quick Start

### Step 1: Create GitHub Repository

1. Go to [github.com/lazyassspecialist-png](https://github.com/lazyassspecialist-png)
2. Click **New repository**
3. Name it exactly: `ayeye.site`
4. Make it **Public**
5. Click **Create repository** (leave it empty)

### Step 2: Push the Site

```bash
cd /home/brpin/workspace/ayeye.site

git init
git add .
git commit -m "Initial ayeye.site — AI side hustle affiliate site"

git remote add origin https://github.com/lazyassspecialist-png/ayeye.site.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your GitHub repo → **Settings** → **Pages**
2. Source: **Deploy from a branch** → **main** → **/ (root)**
3. Click **Save**
4. Wait 2-3 minutes — your site will be live at:
   `https://lazyassspecialist-png.github.io/ayeye.site/`

### Step 4: Point Domain (Later)

Once you're ready for `ayeye.site`:

1. **GitHub:** Settings → Pages → Custom domain: `ayeye.site` → Enforce HTTPS
2. **Namecheap:** DNS settings:
   - Type: `A` | Name: `@` | Value: `185.199.108.153`
   - Type: `CNAME` | Name: `www` | Value: `lazyassspecialist-png.github.io`

GitHub will handle SSL certificate automatically.

---

## 📁 Site Structure

```
ayeye.site/
├── _config.yml          ← Jekyll settings
├── index.md             ← Homepage
├── about.md             ← About page
├── privacy.md           ← Privacy policy
├── _posts/              ← Blog articles (6 published)
│   ├── 2025-04-13-15-best-ai-tools-side-hustles.md
│   ├── 2025-04-13-jasper-ai-review.md
│   ├── 2025-04-13-convertkit-review.md
│   ├── 2025-04-13-thinkific-vs-teachable.md
│   ├── 2025-04-13-semrush-review.md
│   └── 2025-04-13-clickfunnels-review.md
├── _pages/              ← Category pages
│   ├── reviews.md
│   ├── guides.md
│   └── comparisons.md
└── _includes/           ← Reusable components
    └── affiliate-disclosure.html
```

---

## ✏️ Adding New Articles

Create a new file in `_posts/` following this naming convention:

```
YYYY-MM-DD-your-article-title.md
```

Example:
```
2025-04-20-how-to-start-affiliate-marketing.md
```

Required frontmatter (top of every file):
```yaml
---
layout: post
title: "Your Article Title"
category: review  ← use: review, guide, or comparison
excerpt: "One sentence summary for the homepage grid."
date: 2025-04-20
tags: [ai-tools, side-hustle]
---
```

---

## 🔗 Adding Affiliate Links

Every affiliate link needs a disclosure. Use this format:

```markdown
*Disclosure: This article contains affiliate links. We earn a commission
if you purchase through our links, at no extra cost to you.*

[👉 Try Tool Name](https://example.com/affiliate-link) — *Affiliate link*
```

---

## 📊 Next Steps After Setup

1. Apply to affiliate programs (ConvertKit, Jasper AI, Thinkific — easiest approvals)
2. Add Google Analytics or Plausible tracking to `_config.yml`
3. Submit sitemap to Google Search Console
4. Publish 2 more articles per week
5. Apply to Semrush and ClickFunnels affiliate programs

---

## 💡 Content Publishing Schedule

- **Week 1:** Launch articles (6 already done)
- **Week 2:** 2 new articles
- **Week 3:** 2 new articles
- **Week 4:** 2 new articles

Target: 12 articles by end of Month 1. Start appearing in search results by Month 2.

---

*Built with Jekyll + GitHub Pages. Zero hosting costs. Always free.*