# jondevops.dev

Source for [jondevops.dev](https://jondevops.dev), the website of John Paul Babu, a DevOps consultant helping startups and businesses build apps with AI tools on a secure AWS foundation.

Built with [Astro](https://astro.build) as a single static page, with plain CSS and no client-side framework.

## Structure

```text
/
├── public/                  Static files (favicon, photo, CNAME)
├── src/
│   ├── layouts/Layout.astro Page shell and meta tags
│   ├── pages/index.astro    The whole site: content lives at the top of this file
│   └── styles/global.css    Styles (light and dark mode)
└── .github/workflows/       Deploys to GitHub Pages on push to main
```

## Development

Requires Node.js 22 or newer.

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start the dev server at `localhost:4321`    |
| `npm run build`   | Build the site to `./dist/`                 |
| `npm run preview` | Preview the production build locally        |

## Deployment

Pushing to `main` runs the GitHub Actions workflow, which builds the site and publishes it to GitHub Pages. The custom domain is set in `public/CNAME`.

## Contact

[contact@jondevops.dev](mailto:contact@jondevops.dev)
