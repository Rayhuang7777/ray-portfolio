# Personal Website Documentation
**Ray Huang** · Chongqing, China · Class of 2026
`Last updated: June 2025`

---

## 1. Project Overview

This document describes the design, structure, and purpose of my personal website — a single-page portfolio built with HTML, CSS, and JavaScript, hosted on GitHub Pages.

The website is intended to serve as a living portfolio for university applications, collaborative projects, and public engagement. It presents who I am, what I've made, and the questions I'm trying to answer.

**Live URL:** `https://rayhuang7777.github.io`
**Repository:** `https://github.com/Rayhuang7777`

---

## 2. My Identity

| Label | Description |
|---|---|
| **Student of Society** | Interested in the intersection of culture, politics, economics, and youth civic life |
| **Musician & Storyteller** | Lead vocalist and guitarist; uses music and film as modes of expression and inquiry |

---

## 3. Website Goals

The website is designed to:

- Present my personal identity and academic interests to admissions officers, teachers, and collaborators
- Showcase completed and in-progress projects (events, films, photography)
- Share essays and journal entries as evidence of sustained, reflective thinking
- Communicate a coherent worldview: *curious, creative, community-minded, authentic, reflective, driven*
- Serve as a long-term record of work throughout high school and beyond

**First impression I want visitors to have:**
> Curious · Creative · Community-minded · Collaborative · Independent · Authentic · Thoughtful · Driven · Reflective

---

## 4. Design Decisions

### 4.1 Visual Style

| Element | Choice | Reason |
|---|---|---|
| **Overall tone** | Documentary / independent musician | Matches the cultural and journalistic nature of the work |
| **Primary background** | `#1a1917` (charcoal) | Dark, filmic, cinematic — evokes analog photography and live music |
| **Surface color** | `#222220` | Slightly elevated from background for cards and sections |
| **Accent color** | `#b89a6a` (warm sepia) | Single accent only; evokes film grain, aged print, warmth |
| **Muted text** | `#666660` | Low-contrast labels that don't compete with content |
| **Avoided** | Blue, purple, neon gradients | Too digital, too generic — contradicts the analog aesthetic |
| **Background texture** | SVG film grain overlay | Adds depth without image overhead; reinforces documentary feel |

### 4.2 Typography

| Role | Font | Why |
|---|---|---|
| Display / headings | EB Garamond | Cinematic, editorial, classical — used by documentary posters and literary journals |
| Labels / UI | DM Mono | Typewriter feel; evokes film credits, archival documents |
| Body copy | Inter Light | Clean and readable at small sizes without competing with display font |

### 4.3 Interactions

- **Custom cursor** — small amber dot with a lagging ring; reinforces the handcrafted, artisanal feel
- **Scroll-triggered reveals** — sections fade and rise into view as you scroll; creates a sense of gradual discovery
- **Active nav highlighting** — navigation links highlight based on current scroll position via IntersectionObserver
- **Project row hover** — warm sepia wash sweeps across each project row on hover
- **Film grain** — fixed attachment means the grain doesn't scroll, creating a subtle photographic overlay effect

---

## 5. Site Structure

```
rayhuang7777.github.io/
│
├── index-dark.html          ← Main homepage (all sections)
├── photography.html         ← Full photography portfolio page
└── photos/                  ← (To be added) image assets
    ├── hero.jpg
    ├── p1.jpg – p12.jpg
    └── series-*.jpg
```

### 5.1 Homepage Sections

| # | Section | Content |
|---|---|---|
| 1 | **Hero** | Name, headline, tagline, identity badges, CTA |
| 2 | **About** | Personal statement + metadata table |
| 3 | **Projects** | 4 featured projects with tags and descriptions |
| 4 | **Photography** | Mosaic preview + link to full portfolio |
| 5 | **Films** | 2 film entries (one complete, one in production) |
| 6 | **Essays** | 3 essay titles with snippets and dates |
| 7 | **Journal** | 3 short journal entries |
| 8 | **Central Inquiry** | The guiding research question |
| 9 | **Contact** | Email, GitHub, Rednote |

---

## 6. Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Structure and content |
| CSS3 | Layout (CSS Grid, Flexbox), animations, custom properties |
| Vanilla JavaScript | Custom cursor, IntersectionObserver scroll reveals, active nav |
| Google Fonts | EB Garamond, DM Mono, Inter |
| GitHub Pages | Free static hosting with custom domain support |

No frameworks, no build tools, no dependencies. The entire site is a single `.html` file — fast, portable, and easy to maintain.

---

## 7. Content Inventory

### Projects
- [x] Floating Music Festival — Chongqing (2024)
- [x] Youth in the Short-Video Era — documentary (2024)
- [x] Campus Visual Archive — photography (2023–24)
- [x] Model United Nations (2023–25)

### Photography
- [ ] Hero image (needed)
- [ ] 6 mosaic preview photos (needed)
- [ ] 12 full-portfolio photos for photography.html (needed)

### Films
- [ ] Link to completed documentary (coming soon)
- [ ] Behind-the-scenes footage from Floating Music Festival (in production)

### Essays
- [ ] "On Building Stages" — draft exists, needs final edit
- [ ] "What Douyin Is Doing to How We See Ourselves" — draft exists
- [ ] "Culture as Infrastructure" — outline stage

### Journal
- [ ] 3 entries drafted — need to be published as standalone pages or expanded

---

## 8. What I'm Still Working On

- [ ] Upload real photographs to replace all placeholder cells
- [ ] Add hero background image
- [ ] Write and publish 3 essays as full pages
- [ ] Embed or link the short documentary film
- [ ] Add a resume / CV download link
- [ ] Consider adding a Chinese-language toggle for local audiences
- [ ] Register a custom domain (e.g. `rayhuang.me`)

---

## 9. Improvement Suggestions & Update Roadmap

### 9.1 Content to Add (Priority Order)

**High priority — needed for a complete portfolio:**

1. **Real photography** — The single biggest gap. Placeholder cells undermine the visual impact of the whole site. Even 6–8 strong photos transforms the feel entirely.
2. **A downloadable résumé / CV** — Most admissions contexts expect one. A single PDF, linked as a button in the About or Contact section.
3. **Full essay pages** — Right now essays are titles and snippets. Even one full published essay signals intellectual depth. Create `essays/building-stages.html`.
4. **Film embed or link** — A YouTube/Bilibili embed in the Films section turns a description into evidence.

**Medium priority — strengthens the site:**

5. **A brief "Now" page** — A single paragraph about what you're currently reading, listening to, or working on. Updates every few months. Shows the site is alive.
6. **Music section** — A SoundCloud or NetEase embed. You're a musician; the site should sound like you.
7. **More journal entries** — 3 is a start; 8–10 entries over a year makes the journal feel real rather than decorative.

**Lower priority — polish:**

8. **Open Graph meta tags** — So the site looks good when shared on WeChat, WhatsApp, or LinkedIn.
9. **Favicon** — A simple monogram or symbol in the browser tab.
10. **Custom domain** — `rayhuang.me` or `rayhuang.co` costs ~$12/year and looks far more professional than `github.io`.

---

### 9.2 Design Improvements

| Issue | Current State | Suggested Fix |
|---|---|---|
| **Mobile nav** | Links get cramped on small screens | Add a hamburger menu for screens under 640px |
| **Hero without photo** | Feels empty without a background image | Add a real photo, or an abstract graphic made from one of your own shots |
| **Essay pages don't exist yet** | Essay links go nowhere (`href="#"`) | Create individual essay HTML pages or use a simple blog structure |
| **No page transitions** | Clicking links causes a hard page reload | Add a 200ms fade-out on navigation between pages |
| **Photography page filter** | Works, but greying out non-matching photos feels passive | Consider hiding non-matching photos entirely and showing a count ("3 of 12") |
| **No loading state** | Page appears all at once | A very brief (300ms) fade-in on the body prevents a flash of unstyled content |

---

### 9.3 Structural / Strategic Suggestions

**Think of the website in three audiences:**

| Audience | What they want to see | How to serve them |
|---|---|---|
| Admissions officers | Coherent narrative, intellectual depth, evidence of initiative | Strong About page, full essays, central inquiry statement |
| Collaborators / peers | Real work, authentic voice, contact info | Photography, films, journal, responsive email |
| Future self | A record of this period of your life | Keep updating — dates, projects, reflections |

**One sentence per section:**
Each section of your site currently has good content, but consider adding a single italic line under each section heading — a one-sentence personal statement of *why* that section exists. For example, under Photography: *"I photograph what I don't yet know how to write about."*

---

## 10. Reflection

This website is the beginning of a longer project. Right now it presents who I am and what I've done. Over the next year, as the essays get written, the films get finished, and the photographs get taken, it will become something closer to what I actually want: a record of a person trying to understand the world through culture, music, and community.

The central question — *how can culture, creative industries, and public spaces strengthen youth participation and social connection?* — isn't answered here. It's posed. The website is the working document.

---

*Built with HTML, CSS, and JavaScript. Hosted on GitHub Pages. No frameworks were harmed in the making of this site.*
