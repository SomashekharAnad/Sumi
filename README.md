# ✨ Happy Birthday Sumi — Luxury Birthday Website

A cinematic, premium birthday website with Three.js particle fields, GSAP scroll animations, glassmorphism UI, 3D photo cards, infinite gallery strips, memory wall, fireworks finale, and an Easter egg.

---

## 🚀 How to Use

Open `index.html` directly in any modern browser — no build step required.

For the music player to work, you may need to serve from a local server (due to browser audio autoplay policies):

```bash
# Python (any directory)
python3 -m http.server 8080

# Node.js (if installed)
npx serve .
```

Then open `http://localhost:8080`.

---

## ✏️ Customisation Guide

Everything you need to change is in one `CONFIG` block near the top of the `<script>` tag, plus CSS variables in `:root`.

### 1. Name

```js
const CONFIG = {
  name: "Sumi",   // ← Change this
```

Also update the visible text in the HTML where "Sumi" appears in headings.

---

### 2. Photos

Add your image URLs or local paths to the `photos` array:

```js
photos: [
  { src: "assets/images/photo1.jpg", caption: "A Beautiful Smile", date: "Summer 2024" },
  { src: "assets/images/photo2.jpg", caption: "Golden Afternoon",   date: "Autumn 2024" },
  // Add as many as you like — 20+ supported
],
```

Place your images in `/assets/images/`. Supported formats: JPG, PNG, WebP.

> **Tip:** Leave `src: ""` to show a beautiful gradient placeholder with emoji.

---

### 3. Birthday Letter

Find the `#letter` section in the HTML and edit the paragraph text directly:

```html
<p class="letter-para">Your custom message here…</p>
```

---

### 4. Music

```js
music: [
  { src: "assets/music/birthday.mp3", title: "Birthday Serenade" },
  { src: "assets/music/our-song.mp3", title: "Our Song" },
],
```

Place `.mp3` files in `/assets/music/`. The player supports multiple songs and loops automatically.

---

### 5. Colors

Edit CSS custom properties in `:root`:

```css
:root {
  --color-bg:          #050505;   /* page background */
  --color-rose-gold:   #b76e79;   /* primary accent  */
  --color-gold:        #d4a843;   /* gold highlights  */
  --color-pink-soft:   #f4a0b0;
  --color-lavender:    #c8a4d4;
  /* … etc */
}
```

---

### 6. Fonts

Change the Google Fonts `@import` URL and update these variables:

```css
--font-display: 'Playfair Display', serif;
--font-body:    'Cormorant Garamond', serif;
--font-ui:      'Poppins', sans-serif;
```

---

## 🎯 Features

| Feature | Details |
|---|---|
| Loader | Animated gold progress bar with floating sparkles |
| Landing | Star canvas, staggered text, glowing Enter button |
| Three.js Background | 2500-particle gold/rose field + glowing spheres |
| Hero | 4 floating 3D photo cards with mouse parallax tilt |
| Story Timeline | 5-chapter scroll narrative with GSAP triggers |
| Birthday Letter | Scroll-animated paragraphs, glass card |
| Gallery | Dual infinite-scroll strips, lightbox |
| Memory Wall | 3D tilt cards, hover captions |
| Music Player | Floating glass player, progress bar |
| Fireworks | Canvas fireworks + emoji particles in finale |
| Custom Cursor | Heart cursor with trail particles |
| Easter Egg | Type **SUMI** to unlock galaxy animation |
| Responsive | Mobile-first, works on all screen sizes |
| Accessibility | Semantic HTML, ARIA labels, keyboard navigation, reduced motion |

---

## 🗂 Folder Structure

```
sumi-birthday/
├── index.html          ← Everything lives here
├── README.md
└── assets/
    ├── images/         ← Drop your photos here
    │   └── photo1.jpg
    ├── music/          ← Drop your MP3s here
    │   └── birthday.mp3
    ├── icons/
    └── fonts/
```

---

## 🔑 Easter Egg

Type **S → U → M → I** on any keyboard while the site is open. A galaxy animation will unfold. Press **Escape** or click Close to dismiss.

---

## 💌 Made with love
