# StoryCast

StoryCast is a 3-page accessible microsite for audio and video storytelling. It celebrates culture, arts, and the human experience through immersive multimedia narratives.

Built using:
- Semantic HTML5
- Sass (SCSS)
- CSS Grid
- Flexbox
- Container Queries
- WCAG 2.1 AA Accessibility Standards



## Pages

### Home (index.html)
- Hero introduction section
- Featured story highlight
- 6-card responsive story grid
- Mission statement strip

### Story Detail (story/threads-of-time.html)
- Audio player (music preview)
- Story image with caption
- Embedded video with captions
- Transcript section
- Sidebar with structured story metadata

### About / Access (about.html)
- Mission and values
- How stories are produced
- Accessibility statement
- Contact section



## Project Structure

```
/
├── index.html
├── about.html
├── story/
│   └── threads-of-time.html
├── sass/
│   ├── main.scss
│   ├── _colors.scss
│   ├── _typography.scss
│   ├── _spacing.scss
│   ├── _base.scss
│   ├── _layout.scss
│   └── _components.scss
├── css/
│   └── main.css
├── assets/
│   ├── audio/
│   ├── video/
│   └── transcripts/
└── README.md
```

> The CSS is already compiled — no build step is required to run the site.



## Design System

### Colour Palette (Warm & Earthy)

| Token | Hex | Use |
|-------|-----|-----|
| Terracotta | `#c97d4e` | Primary accent & buttons |
| Bark | `#3d2b1f` | Primary text |
| Cream | `#faf6f0` | Page background |
| Ochre | `#d4a853` | Focus ring & highlights |
| Sage | `#6b8f71` | Tags & placeholders |
| Warm Gray | `#b5a495` | Muted labels |

All colour combinations meet WCAG 2.1 AA contrast requirements.

### Typography

| Font | Use |
|------|-----|
| Playfair Display | Headings & titles |
| Lora | Body text |
| Playfair Display SC | Navigation labels |
| Courier Prime | Transcript content |

### Layout & Responsive Strategy

- **CSS Grid** → Page-level layouts (hero, story grid, footer)
- **Flexbox** → Navigation, cards, inline components
- **Container Queries** → Story cards switch layout at 500px container width



## Accessibility Features (WCAG 2.1 AA)

### Media Accessibility
- [x] Full transcript section for audio
- [x] Closed captions (WebVTT) for video
- [x] Audio descriptions track included
- [x] Captions set to default ON
- [x] Fallback text inside `<audio>` and `<video>`
- [x] Downloadable transcript file
- [x] Honest "Coming Soon" note for full documentary

###  Navigation & Interaction
- [x] Skip-to-content link on every page
- [x] Full keyboard accessibility
- [x] 3px visible focus ring
- [x] Accessible mobile navigation with ARIA attributes
- [x] Escape key closes mobile menu
- [x] Breadcrumb navigation
- [x] Keyboard-accessible "Copy Link" button

###  Semantic HTML
- [x] One `<h1>` per page
- [x] Logical heading hierarchy (h1 → h2 → h3)
- [x] Landmark roles (`<header>`, `<main>`, `<footer>`, `<aside>`, `<nav>`)
- [x] Proper use of `<article>`, `<section>`, `<figure>`, `<figcaption>`
- [x] Decorative elements marked `aria-hidden="true"`

###  Motion & Preferences
- [x] `prefers-reduced-motion` supported
- [x] Animations disabled when requested
- [x] No flashing or autoplaying media



##  Media Files Used

| File | Type | Purpose |
|------|------|---------|
| `african_music.mp3` | Audio | Audio preview in player |
| `weaving_process.mp4` | Video | Video section embed |
| `finished_product.jpg` | Image | Story image with caption |

> The audio file is a short preview. The full documentary is marked as "Coming Soon."



## Running Locally

No build step required.

**Option 1 – Python**
```bash
python3 -m http.server 8080
```
Open: http://localhost:8080

**Option 2 – Node**
```bash
npx http-server . -p 8080
```

**Option 3 – VS Code**
Right-click `index.html` → Open with Live Server



## Recompiling Sass (Optional)

Install Sass:
```bash
npm install -g sass
```

Compile:
```bash
sass sass/main.scss css/main.css
```

Watch for changes:
```bash
sass --watch sass/main.scss css/main.css
```



## Browser Support

| Browser | Version |
|---------|---------|
| Chrome | 108+ |
| Firefox | 110+ |
| Safari | 16+ |
| Edge | 108+ |

---

