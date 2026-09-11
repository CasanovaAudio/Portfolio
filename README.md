# Cristian Casanova — Responsive Portfolio

A real, responsive, no-build portfolio website based on the approved cinematic portfolio direction: dark editorial layout, teal accent, full-bleed personal photography, video previews, project modals, audio before/after section, responsive mobile navigation and reusable project data.

## Included real assets
- `assets/hero.jpg` — personal portfolio photo
- `assets/voces-invisibles.mp4` — current project video
- `assets/level-up-thumb.png` — Level Up Mortgages project frame

## Run locally
You can open `index.html` directly, but a local server is recommended for video playback:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Add your own projects
Open `script.js` and add/edit an entry in the `projects` object. For a video project, place the MP4 inside `assets/` and set `media:'video'` and `src:'assets/your-video.mp4'`. For an image, use `media:'image'`.

For a production portfolio with many projects, the same visual system can be migrated to Framer CMS. Framer supports CMS-backed detail pages and video fields, including uploaded files, YouTube, Vimeo and self-hosted video.

## Publish
This static version can be deployed to Netlify, Vercel, GitHub Pages, Cloudflare Pages or any standard static host. If you want a visual CMS instead of editing `script.js`, recreate the design in Framer and use a CMS collection for projects.

## Recommended production media
- Hero image: WebP/JPEG, 2000–2800px wide.
- Portfolio preview loops: H.264 MP4, short and muted.
- Full projects: preferably Vimeo/YouTube or optimized hosted video rather than huge raw files.
- Keep a poster/thumbnail for every video.
