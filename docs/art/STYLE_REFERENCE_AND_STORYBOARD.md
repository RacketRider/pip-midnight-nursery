# PipOS — Master Style Reference & 5-Moment Storyboard
**Track 1: haX.baby 2026 Hackathon | Junior Dream Engineer at Midnight Nursery**
**Author: Gemini Visual Art Director & Production Artist**
**Target Branch: `assets/gemini`**

---

## 1. Visual Identity & Art Direction Lock

### 1.1 Character Canon Lock: Pip
- **Anatomy & Features**: Cute, friendly baby with a smooth, round cream skull face (`#FFF4E7`), soft blush undertones (`#F5C9DC`), large dark round eye sockets with warm, cozy glowing golden starlight (`#FFE5A0`) pinpricks of light in the centers, a tiny crooked smile, and tiny rounded nose.
- **Headgear**: Bedtime sleeping nightcap patterned with golden stars, a fluffy pom-pom, and a signature little pink bow (`#F5C9DC`) on the side.
- **Attire**: Cozy pastel cream and blush pajamas/onesie with heart patterns and soft lavender soles/cuffs.
- **Personality Grammar**: Curious, sleepy, slightly clumsy, and easily delighted. Waving warmly to visitors, holding up the first nightlight filament, and snoozing peacefully.
- **Strict Canon Rule**: Never scary, creepy, or gory. Tactile 3D storybook porcelain, felt, painted wood, and pastel clay qualities.

### 1.2 Color Hierarchy & Palette Architecture
All scenes, SVG icons, and UI chrome strictly adhere to the locked 6-color system from `VISUAL_BIBLE.md`:

| Swatch Role | Name | Hex Code | Scene & UI Application |
| :--- | :--- | :--- | :--- |
| **Surface / Skull / Highlight** | Cream | `#FFF4E7` | Pip's skull face, window cards, readable text panels, moon highlights |
| **Cute Warm Accent** | Blush | `#F5C9DC` | Nightcap pink bow, cheek blush, active buttons, soft cushions |
| **Midtone Magical** | Lavender | `#C9B6E7` | Puffy clouds, window titlebars, secondary panels, bedside trim |
| **Key Light / Focal Glow** | Starlight | `#FFE5A0` | Glowing eye pinpricks, lanterns, stars, path routes, cursor sparkles |
| **Structural Line / Outline** | Plum | `#81638E` | 2px window borders, illustration linework, bevel drop shadows |
| **Primary Dark / Ambient Sky** | Midnight | `#25233F` | Night sky, dark-mode wainscoting, room shadows, primary body copy on Cream |

### 1.3 Material Qualities & Lighting Logic
- **Tactile Materials**: Soft porcelain, felt, painted wood, delicate fabric, and pastel clay-like textures. Smooth rounded curves, gentle contact shadows, and warm glowing lamps.
- **Early-2000s OS Chrome**: 16px rounded window corners, 2px solid Plum (`#81638E`) borders, 2px Cream (`#FFF4E7`) inner top-left bevel highlights, 32px Lavender titlebars with Star, Moon, and Bow faux-OS pills, and 4px 4px 0px `#25233F` retro drop shadows.
- **Single-Source Warm Lighting**: Every scene is illuminated by warm golden Starlight (`#FFE5A0`) radiating from lanterns and stars, casting velvety Midnight (`#25233F`) shadows and soft Lavender (`#C9B6E7`) ambient fill.
- **Zero Baked-In Text**: No interface words, buttons, or fake OS text are embedded in any raster or vector art. All typography is rendered cleanly in live HTML/CSS.

---

## 2. Connected 5-Moment Storyboard

The site unfolds along a continuous vertical narrative journey inside the Midnight Nursery:

```
[ MOMENT 1: WELCOME ] -> [ MOMENT 2: ORIGIN ] -> [ MOMENT 3: WORKSHOP ] -> [ MOMENT 4: NIGHTLIGHT ] -> [ MOMENT 5: GOODNIGHT ]
```

### Moment 1: WELCOME (The PipOS Magical Desktop)
- **Narrative**: The desktop boots up. Pip waves hello from a puffy cloud perch, introduces themself as Junior Dream Engineer at Midnight Nursery, and displays the tagline: *"I build the dreams you fall asleep inside."*
- **Visual Staging**: 
  - Background: `scenes/desktop-bg.webp` (Desktop) / `scenes/desktop-bg-mobile.webp` (Mobile) showing the cozy nursery workshop with arched starry window.
  - Character: `character/pip-hero.webp` waving warmly on a fluffy cloud with true alpha transparency.
- **Desktop (1440×900)**: Left/Center-Left (x: 8%–52%) hosts the rounded Cream/Lavender HTML Welcome window and 3 desktop launcher tiles (`icon-lullaby.svg`, `icon-nightlight.svg`, `icon-delivery.svg`). Right Stage (x: 54%–90%) showcases `pip-hero.webp` with plenty of breathing room.
- **Mobile (390×844)**: Top Stage (y: 8%–46%) showcases `pip-hero.webp`; lower half (y: 48%–84%) docks the full-width stacked Welcome card above the bottom launcher dock.

### Moment 2: ORIGIN (From Dim Star to Midnight Nursery)
- **Narrative**: Three-beat scroll-driven origin story:
  - **Beat 2A**: A lonely, dim star in a quiet Midnight sky where little creatures couldn't fall asleep.
  - **Beat 2B**: Pip invents a first warm light (`scenes/origin-workshop.webp` + `character/pip-story.webp`).
  - **Beat 2C**: Signature Moment #2 — `scenes/origin-star.svg` animates `#constellation-threads` into a glowing Starlight constellation crowning the Midnight Nursery.
- **Desktop (1440×900)**: Left/Center (x: 10%–58%) displays the framed `origin-workshop.webp` with `origin-star.svg` overlay; Right (x: 62%–90%) displays 3 concise story caption cards.
- **Mobile (390×844)**: Sticky upper visual stage (y: 10%–50%) displays the animated constellation over `origin-workshop.webp`, while the 3 short HTML story cards scroll cleanly below (y: 52%–86%).

### Moment 3: WORKSHOP (The 3-Project Desktop Hub)
- **Narrative**: Pip's dream-making workbench with three playable, accessible projects:
  1. **Lullaby Lab**: Wind-up music box (`projects/musicbox.webp`) with interactive pastel chimes, animated star notes, and working audio mute toggle.
  2. **Nightlight Collection**: Room illumination showcase (`projects/lantern.webp` + `projects/nightlight-room.webp`).
  3. **Dream Delivery**: Interactive rooftop map (`projects/dream-map.svg`) connecting the Midnight Nursery to 3 neighbourhood houses.
- **Desktop (1440×900)**: Left dock (x: 6%–22%) features 3 large tactile desktop icon buttons with labels; Center-Right (x: 24%–92%) opens one accessible project window at a time.
- **Mobile (390×844)**: Active project fills a clean full-width card (y: 8%–80%); bottom 64px is reserved for the fixed thumb-friendly project launcher dock.

### Moment 4: NIGHTLIGHT INTERACTION (Signature Light-Reveal Experience)
- **Narrative**: Signature Moment #1 — The visitor uses Pip's Dream Lantern (`projects/lantern.webp`) to illuminate a darkened nursery bedroom (`projects/nightlight-room.webp`) to discover 4 cozy secrets:
  1. Bottom-left: Cute smiling baby ghost plushie under the crib.
  2. Upper-left shelf: Glowing glass dream-jars and star rattle blocks.
  3. Center-right rug: Friendly lavender baby monster sleeping under a quilt.
  4. Far-right window nook: Sleeping crescent moon cushion with a pink bow.
- **Pixel-Aligned Implementation**: One single base image (`nightlight-room.webp`). Layer 1 is darkened via CSS (`filter: brightness(0.22) saturate(0.65) hue-rotate(-12deg)`), while Layer 2 is identical at 100% warm brightness inside a dynamic CSS `mask-image: radial-gradient(...)` following pointer, touch, or keyboard jump buttons.

### Moment 5: GOODNIGHT (System Sleep & Secret Moon Easter Egg)
- **Narrative**: The nursery dims to deep Midnight (`#25233F`). Pip sleeps peacefully under a soft lullaby glow. Clicking or activating the glowing crescent moon (`ui/moon.svg`) unlocks the Secret Dream modal (`easter-egg/secret-dream.webp`): Pip and baby ghost friends having a cloud-castle star-cookie slumber party.
- **Desktop (1440×900)**: Top-right sky (x: 74%–86%, y: 12%–28%) features the interactive `moon.svg` with twinkle halo; Center-Left (x: 15%–52%) shows sleeping Pip; Right (x: 54%–88%) frames the Credits & Replay card.
- **Mobile (390×844)**: Top Center (y: 10%–22%) features the large tappable `moon.svg`; Middle (y: 24%–54%) showcases sleeping Pip; Lower stage (y: 56%–86%) contains compact credits and "Back to Top" button.

---

## 3. Production Asset Inventory (`public/assets/...`)

All 16 production assets have been authored, optimized, and verified in `public/assets/`:

| Manifest Path | Format & Mode | Dimensions / viewBox | Storyboard Moment | Description & Technical Notes |
| :--- | :--- | :--- | :--- | :--- |
| `character/pip-hero.webp` | WebP (RGBA Transparent) | 1024×1024 px (1:1) | 1 (Welcome) | Canon Pip waving warmly on fluffy cloud, clear silhouette, true alpha. |
| `character/pip-story.webp` | WebP (RGBA Transparent) | 1024×1024 px (1:1) | 2, 3 (Origin, Workshop) | Pip in 3/4 pose holding the first light filament, true alpha. |
| `scenes/desktop-bg.webp` | WebP (RGB) | 2880×1620 px (16:9) | 1, 3, 5 (Desktop Shell) | Panoramic nursery workshop with arched starry window, 65% calm UI space. |
| `scenes/desktop-bg-mobile.webp` | WebP (RGB) | 1170×2080 px (9:16) | 1, 3, 5 (Mobile Shell) | Vertical nursery framing for 390×844 mobile stacking, zero baked-in UI. |
| `scenes/origin-workshop.webp` | WebP (RGB) | 1600×900 px (16:9) | 2 (Origin Beat 2B) | Cozy nursery workbench with first nightlight in glass dome & calipers. |
| `scenes/origin-star.svg` | SVG (Vector) | `viewBox="0 0 800 500"` | 2 (Origin Beat 2A–2C) | Layered SVG with animatable `#constellation-threads` & `#origin-primary-star`. |
| `projects/musicbox.webp` | WebP (RGB) | 1024×924 px | 3 (Workshop: Lullaby) | Official-derived pastel unicorn wind-up music box with golden key. |
| `projects/lantern.webp` | WebP (RGB) | 1024×914 px | 3, 4 (Nightlight) | Official-derived glowing crescent moon bedside lantern with brass ring. |
| `projects/nightlight-room.webp` | WebP (RGB) | 1920×1080 px (16:9) | 4 (Nightlight Reveal) | Single fully-lit bedroom with 4 hidden curiosities for CSS spotlight mask. |
| `projects/dream-map.svg` | SVG (Vector) | `viewBox="0 0 1200 750"` | 3 (Workshop: Delivery) | Fixed-viewBox rooftop map with Nursery hub (`600,640`) and 3 house pins. |
| `ui/icon-lullaby.svg` | SVG (Vector) | `viewBox="0 0 64 64"` | 1, 3 (Launchers) | Matching icon: music box with floating golden musical note. |
| `ui/icon-nightlight.svg` | SVG (Vector) | `viewBox="0 0 64 64"` | 1, 3 (Launchers) | Matching icon: dream lantern with starlight halo. |
| `ui/icon-delivery.svg` | SVG (Vector) | `viewBox="0 0 64 64"` | 1, 3 (Launchers) | Matching icon: winged dream letter with starlight trail. |
| `ui/star.svg` | SVG (Vector) | `viewBox="0 0 48 48"` | All (Motifs) | 4-point twinkle star motif with inner highlight and 2px Plum stroke. |
| `ui/moon.svg` | SVG (Vector) | `viewBox="0 0 48 48"` | 5 (Goodnight / Secret) | Sleeping crescent moon with pink ribbon bow and rosy blush. |
| `easter-egg/secret-dream.webp` | WebP (RGB) | 1200×900 px (4:3) | 5 (Goodnight Easter Egg) | Secret slumber party in cloud-castle with friendly baby ghosts & cookies. |

---

## 4. Technical Integration Instructions for Coding Agents (Hermes A & Hermes B)

### 4.1 Nightlight Single-Image Masking (Pixel-Perfect Alignment)
Place this exact CSS in `src/styles/` or component styles:
```css
.nightlight-stage {
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 9;
  border-radius: 16px;
  border: 2px solid #81638E;
  overflow: hidden;
  background: #25233F;
  --spot-x: 50%;
  --spot-y: 50%;
  --spot-radius: 180px;
}

/* Layer 1: Darkened base plate */
.nightlight-room-dark {
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: brightness(0.22) saturate(0.65) contrast(1.1) hue-rotate(-12deg);
}

/* Layer 2: 100% warm lit reveal plate with radial mask */
.nightlight-room-lit {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  pointer-events: none;
  -webkit-mask-image: radial-gradient(
    circle var(--spot-radius) at var(--spot-x) var(--spot-y),
    rgba(0, 0, 0, 1) 0%,
    rgba(0, 0, 0, 0.85) 55%,
    rgba(0, 0, 0, 0) 100%
  );
  mask-image: radial-gradient(
    circle var(--spot-radius) at var(--spot-x) var(--spot-y),
    rgba(0, 0, 0, 1) 0%,
    rgba(0, 0, 0, 0.85) 55%,
    rgba(0, 0, 0, 0) 100%
  );
}
```

### 4.2 Dream Delivery Rooftop Coordinates (`projects/dream-map.svg`)
Fixed coordinates inside `viewBox="0 0 1200 750"`:
- **Origin Hub** (`#hub-midnight-nursery`): `cx="600" cy="640"`
- **House 1** (`#house-1-cottage` — Little Ghost Cottage): `cx="220" cy="360"` | Path ID: `#route-house-1`
- **House 2** (`#house-2-observatory` — CloudSlumber Tower): `cx="600" cy="175"` | Path ID: `#route-house-2`
- **House 3** (`#house-3-burrow` — Cozy Monster Burrow): `cx="980" cy="360"` | Path ID: `#route-house-3`

Animate the chosen path using CSS `stroke-dashoffset` or Motion `pathLength: [0, 1]`.

### 4.3 Origin Constellation Threads Animation (`scenes/origin-star.svg`)
- Animate `#constellation-threads` from `stroke-dashoffset: 1000` to `0` as the user scrolls from Beat 2A to 2C.
- Transition `#constellation-secondary-stars` from `opacity: 0` to `1`.
