# 🍕 Barcelona Pizza Blog - LIVE

## ✅ Status: DEPLOYED & WORKING

**Live Website**: https://fiddi-clawbot.github.io/barcelona-pizza/

---

## 🎨 Design
- **Theme**: Dark modern (midnight blue background, orange accent)
- **Responsive**: Mobile, tablet, desktop all optimized
- **Colors**: 
  - Background: `#0f1419` 
  - Text: `#e8eaed`
  - Accent: `#ff6b35`
- **Components**: Hero section, card grid, detail pages, gallery

---

## 🍽️ Featured Pizzerias

### 1. **Pizzeria Beddia** (Eixample)
- **Award**: Michelin Recognition (2023)
- **Style**: Neapolitan
- **Specialty**: 72-hour fermented dough, imported mozzarella
- **Details**: [View →](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/beddia/)

### 2. **Franco Pepe** (Gràcia)
- **Award**: Forbes Pick 2024
- **Style**: Regional Italian (Umbrian)
- **Specialty**: Local sourcing, seasonal ingredients
- **Details**: [View →](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/franco-pepe/)

### 3. **Pizzeria Al Taglio** (Born)
- **Award**: Timeout Featured (2023)
- **Style**: Roman (al taglio)
- **Specialty**: Gabriele Bonci's technique, daily cuts
- **Details**: [View →](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/al-taglio/)

### 4. **Can Culleretes** (Gothic Quarter)
- **Award**: Barcelona's Oldest Restaurant (1786)
- **Style**: Traditional Catalan-Italian Fusion
- **Specialty**: Heritage approach, seasonal dishes
- **Details**: [View →](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/can-culleretes/)

### 5. **Pizzeria Lo Grec** (Sarrià-Sant Gervasi)
- **Award**: Michelin Bib Gourmand (2023)
- **Style**: Modern Neapolitan
- **Specialty**: Barcelona ingredients + Italian tradition
- **Details**: [View →](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/lo-grec/)

---

## 🛠️ Infrastructure

**Tech Stack:**
- **Framework**: Jekyll (static site generator)
- **Hosting**: GitHub Pages (free, fast, secure)
- **Deployment**: GitHub Actions (automated)
- **CSS**: Custom dark theme, responsive grid
- **Domain**: GitHub Pages subdomain

**How It Works:**
1. Content written in Markdown (`_pizzerias/*.md`)
2. Jekyll builds HTML from templates
3. GitHub Actions automated the build on every push
4. Built files deployed to `gh-pages` branch
5. GitHub Pages serves from gh-pages automatically

---

## 📝 Content Structure

Each pizzeria page includes:
- ✅ Hero image
- ✅ Name, location, cuisine type
- ✅ Award/recognition badge
- ✅ Story (2-3 paragraphs)
- ✅ Signature pizza description
- ✅ Image gallery (2 photos)
- ✅ Website link
- ✅ Google Maps link
- ✅ Address & hours

---

## 📂 Repository

**GitHub**: https://github.com/fiddi-clawbot/barcelona-pizza

**Structure:**
```
barcelona-pizza/
├── _pizzerias/          # Pizzeria content (Markdown)
│   ├── beddia.md
│   ├── franco-pepe.md
│   ├── al-taglio.md
│   ├── can-culleretes.md
│   └── lo-grec.md
├── _layouts/            # HTML templates
│   ├── default.html
│   └── pizzeria.html
├── assets/
│   ├── css/style.css    # Dark theme styles
│   └── images/          # Placeholder images
├── _config.yml          # Jekyll configuration
├── Gemfile              # Ruby dependencies
├── index.md             # Home page
├── pizzerias.md         # Directory page
└── .github/workflows/   # GitHub Actions
    └── jekyll.yml       # Build automation
```

---

## 🚀 Next Steps (Optional)

1. **Better Images**: Replace placeholders with real pizzeria photos
2. **Custom Domain**: Point your own domain to the site
3. **Analytics**: Add Google Analytics
4. **Comments**: Add Disqus or Utterances for reader feedback
5. **Expand**: Add 5-10 more pizzerias
6. **SEO**: Optimize meta descriptions, alt text
7. **Features**: Add search, filtering, ratings

---

## 💡 How to Update

**To add a new pizzeria:**

1. Create a new markdown file in `_pizzerias/name.md`
2. Fill in the frontmatter (name, award, etc.)
3. Add the story content
4. Push to GitHub
5. GitHub Actions automatically rebuilds and deploys

**To modify design:**

1. Edit `assets/css/style.css`
2. Push to GitHub
3. Site automatically rebuilds

**Example pizzeria file:**
```markdown
---
name: Pizzeria Name
neighborhood: Neighborhood
cuisine: Style
award: Award (2024)
teaser: Short description
image: /barcelona-pizza/assets/images/name.jpg
website: https://example.com
google_maps: https://maps.google.com/...
---

# Pizzeria Name

## The Story
[Content here...]

## Signature Pizza
[Description here...]
```

---

**Status**: ✅ LIVE & READY
**Build Time**: ~2 minutes
**Deploy**: Automatic on push
**Performance**: Fast (static HTML)
**Hosting Cost**: FREE (GitHub Pages)

Enjoy! 🍕
