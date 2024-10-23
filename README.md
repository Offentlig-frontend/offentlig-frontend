## Offentlig frontend homepage

This is the officially sanctioned repository for the offentlig frontend website. Offentlig frontend is loose collaboration for frontend developers in public organisations on Norway.

As per now, the project is implemented in Astro.

### Deployment

Project deployment is setup on vercel on a personal account. Merges to the `astro` branch is automatically deployed to https://offentlig-frontend-beta.vercel.app/ to avoid possible clashes with the existing website on https://offentlig-frontend.vercel.app/. This is likely to change soon.

But for now, all new development should be merged to the `astro` branch.

### File structure of the project

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

### 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
