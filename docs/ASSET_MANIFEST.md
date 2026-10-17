# Asset pipeline and authoritative filenames

## Authoritative delivery path
All approved final assets live in public/assets/. No remote Gemini links in app code. Commit assets through assets/gemini PRs; keep a local source-art archive outside the app if source artwork is large.

## Manifest (Delivery Status)
- `character/pip-hero.webp` [DELIVERED]: 1024×1024 px, WebP (RGBA True Transparency), official-derived canon character waving on cloud, clear silhouette.
- `character/pip-story.webp` [DELIVERED]: 1024×1024 px, WebP (RGBA True Transparency), consistent Pip 3/4 pose holding the first light filament.
- `scenes/desktop-bg.webp` [DELIVERED]: 2880×1620 px (16:9, covers 1440×900 @ 2x), WebP (RGB), panoramic Midnight Nursery with starry arched window and 65% calm negative space for UI windows.
- `scenes/desktop-bg-mobile.webp` [DELIVERED]: 1170×2080 px (9:16, covers 390×844 @ 3x), WebP (RGB), mobile-safe vertical nursery framing.
- `scenes/origin-star.svg` [DELIVERED]: viewBox="0 0 800 500", clean layered vector artwork with animatable `#constellation-threads` and `#constellation-secondary-stars`.
- `scenes/origin-workshop.webp` [DELIVERED]: 1600×900 px (16:9), WebP (RGB), cozy nursery drafting workbench with first warm nightlight in glass dome.
- `projects/musicbox.webp` [DELIVERED]: 1024×924 px, WebP, official-derived pastel unicorn wind-up music box.
- `projects/lantern.webp` [DELIVERED]: 1024×914 px, WebP, official-derived glowing crescent moon bedside lantern.
- `projects/nightlight-room.webp` [DELIVERED]: 1920×1080 px (16:9), WebP (RGB), single fully-lit room with 4 hidden curiosities for CSS-darkened base + radial spotlight mask.
- `projects/dream-map.svg` [DELIVERED]: viewBox="0 0 1200 750", illustrated rooftop map with 3 fixed house anchor coordinates and 3 delivery route paths.
- `ui/icon-lullaby.svg` [DELIVERED]: viewBox="0 0 64 64", matching music box launcher icon with 2px Plum stroke.
- `ui/icon-nightlight.svg` [DELIVERED]: viewBox="0 0 64 64", matching lantern launcher icon with 2px Plum stroke.
- `ui/icon-delivery.svg` [DELIVERED]: viewBox="0 0 64 64", matching winged dream letter launcher icon with 2px Plum stroke.
- `ui/star.svg` [DELIVERED]: viewBox="0 0 48 48", 4-point twinkle star motif with inner highlight.
- `ui/moon.svg` [DELIVERED]: viewBox="0 0 48 48", sleeping crescent moon with pink ribbon bow (Easter egg trigger).
- `easter-egg/secret-dream.webp` [DELIVERED]: 1200×900 px (4:3), WebP (RGB), Pip and baby ghost friends having a cloud-castle star-cookie slumber party.

## Generation consistency protocol
Start with official Pip portrait and a single signed-off style reference. For EACH subsequent generated scene, reuse those inputs as references and reiterate consistent Pip anatomy, shape, cap, lighting, materials, edge treatment and palette. Reject inconsistent characters rather than trying to hide them in CSS.

## VERY IMPORTANT: Nightlight alignment
Do NOT ask Gemini to separately regenerate a dark and light room. Independent generation often shifts objects. Generate ONE light/base room scene. In CSS place that identical image as a masked bright layer over the same image darkened by CSS. This guarantees pixel alignment.

## Exports
No text or UI labels baked into art. Separate independently animated layers where practical. SVG for maps and icons; optimized WebP for backgrounds and raster figures. Document dimension or viewBox, transparency, version, source, and license/attribution. Keep image formats readable across target browsers.

## Gemini handoff
The operator reviews generation, renames file to manifest name, checks crop/transparency, previews on desktop/mobile, uploads via assets/gemini branch. Each asset PR includes a preview collage plus what it replaces. Hermes A merges, then Hermes B updates feature branch from main.

## Official reference pack
https://hax.baby/baby/assets/track1-pip-asset-pack.zip
https://hax.baby/baby/assets/pip_portrait.png
https://hax.baby/baby/assets/pip_avatar_cloud.png
https://hax.baby/baby/assets/pip_lullaby_box.png
https://hax.baby/baby/assets/pip_dream_lantern.png
