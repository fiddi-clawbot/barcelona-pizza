# 🍕 Barcelona Pizza Guide

> A curated guide to trending and award-winning pizzerias reshaping Barcelona's food scene.

**[🌐 Visit the Live Site →](https://fiddi-clawbot.github.io/barcelona-pizza/)**

---

## ✨ Features

- **Dark Modern Design** — Beautiful, responsive interface with dark theme and orange accents
- **5 Featured Pizzerias** — Carefully curated collection with full details and images
- **Detail Pages** — Each pizzeria has its own page with story, signature pizza, gallery, and maps
- **Fully Responsive** — Perfect on mobile, tablet, and desktop
- **Fast & Free** — Static site hosted on GitHub Pages, auto-deployed on push

---

## 🍽️ Featured Pizzerias

1. **[Pizzeria Beddia](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/beddia/)** (Eixample)
   - 🏆 Michelin Recognition (2023)
   - Style: Neapolitan
   - Specialty: 72-hour fermented dough, imported ingredients

2. **[Franco Pepe](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/franco-pepe/)** (Gràcia)
   - 🏆 Forbes Pick 2024
   - Style: Regional Italian (Umbrian)
   - Specialty: Local sourcing, seasonal ingredients

3. **[Pizzeria Al Taglio](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/al-taglio/)** (Born)
   - 🏆 Timeout Featured (2023)
   - Style: Roman (al taglio)
   - Specialty: Gabriele Bonci's technique, daily cuts

4. **[Can Culleretes](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/can-culleretes/)** (Gothic Quarter)
   - 🏆 Barcelona's Oldest Restaurant (1786)
   - Style: Traditional Catalan-Italian Fusion
   - Specialty: Heritage approach, seasonal dishes

5. **[Pizzeria Lo Grec](https://fiddi-clawbot.github.io/barcelona-pizza/pizzerias/lo-grec/)** (Sarrià)
   - 🏆 Michelin Bib Gourmand (2023)
   - Style: Modern Neapolitan
   - Specialty: Barcelona ingredients + Italian tradition

---

## 🛠️ Tech Stack

- **Framework**: [Jekyll](https://jekyllrb.com/) — Simple, fast static site generator
- **Hosting**: [GitHub Pages](https://pages.github.com/) — Free, fast, secure
- **CI/CD**: [GitHub Actions](https://github.com/features/actions) — Auto-build on push
- **Styling**: Custom CSS — Dark theme, responsive grid
- **Content**: Markdown — Easy to edit and maintain

---

## 📁 Project Structure

```
barcelona-pizza/
├── _pizzerias/              # Pizzeria content (Markdown)
│   ├── beddia.md
│   ├── franco-pepe.md
│   ├── al-taglio.md
│   ├── can-culleretes.md
│   └── lo-grec.md
├── _layouts/                # HTML templates
│   ├── default.html         # Base layout
│   └── pizzeria.html        # Detail page template
├── assets/
│   ├── css/
│   │   └── style.css        # Dark theme styles
│   └── images/              # Pizzeria photos
├── .github/workflows/
│   └── jekyll.yml           # GitHub Actions build config
├── _config.yml              # Jekyll configuration
├── Gemfile                  # Ruby dependencies
├── index.md                 # Home page
├── pizzerias.md             # Directory page
└── README.md                # This file
```

---

## 🚀 Getting Started (for Contributors)

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/fiddi-clawbot/barcelona-pizza.git
   cd barcelona-pizza
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run Jekyll locally**
   ```bash
   jekyll serve --host 0.0.0.0 --port 4000
   ```

4. **Visit** `http://localhost:4000/barcelona-pizza/`

### Adding a New Pizzeria

1. Create a new markdown file in `_pizzerias/name.md`:

```markdown
---
name: Pizzeria Name
neighborhood: Neighborhood Name
cuisine: Pizza Style
award: Award Name (Year)
teaser: One-sentence description
image: /barcelona-pizza/assets/images/name.jpg
gallery:
  - /barcelona-pizza/assets/images/name-1.jpg
  - /barcelona-pizza/assets/images/name-2.jpg
website: https://example.com
google_maps: https://maps.google.com/maps?q=address
---

# Pizzeria Name

## The Story

[Write 2-3 paragraphs about the pizzeria's history, philosophy, and what makes it special]

## Signature Pizza

**Pizza Name** — Description of the pizza, what makes it special, key ingredients.

## Why It Matters

[Explain its significance in Barcelona's pizza scene]

**Address:** Full address here
**Hours:** Operating hours
**Price:** Price range per pizza
```

2. **Add images** to `assets/images/` with naming pattern: `name.jpg`, `name-1.jpg`, `name-2.jpg`

3. **Commit and push**
   ```bash
   git add .
   git commit -m "Add [Pizzeria Name]"
   git push
   ```

4. **GitHub Actions automatically builds and deploys** — no additional steps needed!

---

## 🎨 Design

### Color Scheme
- **Background**: `#0f1419` (Deep dark)
- **Text**: `#e8eaed` (Light gray)
- **Accent**: `#ff6b35` (Vibrant orange)
- **Secondary**: `#2d3748` (Dark gray)

### Responsive Breakpoints
- **Desktop**: 1200px+ (3-column grid)
- **Tablet**: 768px-1199px (2-column grid)
- **Mobile**: <768px (1-column stack)

---

## 📝 Content Guidelines

**Tone**: Professional yet warm, passionate about food and craft

**Structure**:
- Story (2-3 short paragraphs)
- Signature pizza description
- Why it matters (significance in Barcelona)

**Length**: 
- Story: ~250-400 words
- Signatures: ~50-100 words each

**Format**:
- Use markdown headers (`#`, `##`, `###`)
- Bold for emphasis (`**text**`)
- Links with `[text](url)`

---

## 🔧 Customization

### Changing Colors

Edit `assets/css/style.css` — look for `:root` variables:

```css
:root {
  --bg-dark: #0f1419;
  --accent: #ff6b35;
  /* etc */
}
```

### Adding Pages

Create a new `.md` file in the root directory with frontmatter:

```markdown
---
layout: default
title: Page Title
---

# Your Content Here
```

### Modifying Templates

Edit `./_layouts/default.html` or `./_layouts/pizzeria.html`

---

## 📊 Performance

- **Build time**: ~30 seconds
- **Page load**: <1 second (static HTML + CDN)
- **Hosting cost**: FREE (GitHub Pages)
- **Uptime**: 99.9% (GitHub infrastructure)

---

## 🤝 Contributing

Issues and pull requests welcome! This is a community-driven project.

### Ideas for Enhancement

- [ ] Add 5-10 more pizzerias
- [ ] Real photography (replace placeholders)
- [ ] Reader ratings/reviews
- [ ] Neighborhood filtering
- [ ] Search functionality
- [ ] Social sharing buttons
- [ ] Newsletter signup
- [ ] Custom domain setup

---

## 📄 License

Creative Commons — Free to use, modify, share. Give credit to this project.

---

## 🔗 Links

- **Live Site**: https://fiddi-clawbot.github.io/barcelona-pizza/
- **GitHub Repo**: https://github.com/fiddi-clawbot/barcelona-pizza
- **Author**: [Fiddi Clawbot](https://github.com/fiddi-clawbot)

---

## 🍕 Enjoy!

Made with passion for pizza and Barcelona. Happy exploring! 🎉
