# Creative Web Universe

A living archive of **15 distinct digital worlds** — a premium showcase of art direction, interaction and frontend craft. Each project has its own atmosphere, palette and editorial voice while sharing a clear navigation system.

## Stack

- React 19 + TypeScript
- Vite 8
- React Router
- Lucide React icons
- CSS custom properties, responsive grid and motion
- Fixed Unsplash image assets for visual studies

## The collection

| # | Project | World |
|---|---|---|
| 01 | Neural | Future / Technology |
| 02 | Nexus | Future / Technology |
| 03 | Quantum | Future / Technology |
| 04 | Orbit | Future / Technology |
| 05 | Synapse | Future / Technology |
| 06 | Monument | Culture / Creative |
| 07 | Noir | Culture / Creative |
| 08 | Aether | Culture / Creative |
| 09 | Lumen | Culture / Creative |
| 10 | Pulse | Culture / Creative |
| 11 | Atelier | Business / Premium |
| 12 | Savor | Business / Premium |
| 13 | Forma | Business / Premium |
| 14 | North | Business / Premium |
| 15 | Velaris | Business / Premium |

## Run locally

```bash
npm install
npm run dev
```

Then open the local URL shown by Vite. For a production build:

```bash
npm run build
npm run preview
```

## Structure

```text
src/
├── data/projects.ts   # Typed content model and 15 project records
├── App.tsx            # Home, detail views, navigation and interactions
├── index.css          # Visual system, responsive layout and animations
└── main.tsx           # React entrypoint and BrowserRouter
```

## Adding a new project

Add a new typed record to `src/data/projects.ts`. Include an `id`, `route`, `category`, copy, accent colors, image and tags. The showcase cards and detail route are generated from that data automatically.

## Deploy

The app is a static Vite build and can be deployed to Vercel, Netlify or GitHub Pages. Build with `npm run build` and serve the generated `dist/` directory. If deploying to a platform with history fallback disabled, configure all routes to serve `index.html` so project paths work on refresh.

## Design notes

The home page uses an editorial asymmetric grid, three category filters, motion-reduced CSS transitions, a mobile menu and a responsive detail template. Images are loaded lazily on the collection to keep the first paint light.
