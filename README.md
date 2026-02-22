## StoryCast

StoryCast is a 3-page accessible microsite for audio and video storytelling.
It celebrates culture, arts, and the human experience through immersive multimedia narratives.

Built using:

Semantic HTML5

Sass (SCSS)

CSS Grid

Flexbox

Container Queries

WCAG 2.1 AA Accessibility Standards

Pages
Home (index.html)

Hero introduction section

Featured story highlight

6-card responsive story grid

Mission statement strip

Story Detail (story/threads-of-time.html)

Audio player (music preview)

Story image with caption

Embedded video with captions

Transcript section

Sidebar with structured story metadata

About / Access (about.html)

Mission and values

How stories are produced

Accessibility statement

Contact section

Project Structure
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

The CSS is already compiled — no build step is required to run the site.

Design System
Colour Palette (Warm & Earthy)

Terracotta (#c97d4e) – Primary accent & buttons

Bark (#3d2b1f) – Primary text

Cream (#faf6f0) – Page background

Ochre (#d4a853) – Focus ring & highlights

Sage (#6b8f71) – Tags & placeholders

Warm Gray (#b5a495) – Muted labels

All colour combinations meet WCAG 2.1 AA contrast requirements.

Typography

Playfair Display – Headings & titles

Lora – Body text

Playfair Display SC – Navigation labels

Courier Prime – Transcript content

Layout & Responsive Strategy

CSS Grid → Page-level layouts (hero, story grid, footer)

Flexbox → Navigation, cards, inline components

Container Queries → Story cards switch layout at 500px container width

Accessibility Features (WCAG 2.1 AA)
Media Accessibility

Full transcript section for audio

Closed captions (WebVTT) for video

Audio descriptions track included

Captions set to default ON

Fallback text inside <audio> and <video>

Downloadable transcript file

Honest “Coming Soon” note for full documentary

⌨ Navigation & Interaction

Skip-to-content link on every page

Full keyboard accessibility

3px visible focus ring

Accessible mobile navigation with ARIA attributes

Escape key closes mobile menu

Breadcrumb navigation

Keyboard-accessible “Copy Link” button

Semantic HTML

One <h1> per page

Logical heading hierarchy

Landmark roles (<header>, <main>, <footer>)

Proper use of <article>, <section>, <figure>, <aside>

Decorative elements marked aria-hidden="true"

Motion & Preferences

prefers-reduced-motion supported

Animations disabled when requested

No flashing or autoplaying media

🎬 Media Files Used

african_music.mp3 → Audio preview

weaving_process.mp4 → Video section

finished_product.jpg → Story image

The audio file is a short preview. The full documentary is marked as “Coming Soon.”

Running Locally

No build step required.

Option 1 – Python
python3 -m http.server 8080

Open: http://localhost:8080

Option 2 – Node
npx http-server . -p 8080
Option 3 – VS Code

Right-click index.html → Open with Live Server

Recompiling Sass (Optional)

Install Sass:

npm install -g sass

Compile:

sass sass/main.scss css/main.css

Watch for changes:

sass --watch sass/main.scss css/main.css
Browser Support

Chrome 108+

Firefox 110+

Safari 16+

Edge 108+
