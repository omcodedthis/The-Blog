# The-Blog
The source code for my blog, named 'The Blog' which is built using [Astro](https://astro.build/). Astro is an open-source, server-first web framework that combines the best of static site generation (SSG) and server-side rendering (SSR) to create fast, SEO-friendly websites. `My-Blog` (named as 'The Blog') is built using this [Astro template](https://github.com/satnaing/astro-paper).

### [The website is now live!](https://omsblog.pages.dev/)

## Project Structure

The file structure is as follows:

```bash
/
├── public/
│   ├── assets/
│   │   └── logo.svg
│   │   └── logo.png
│   └── favicon.svg
│   └── astropaper-og.jpg
│   └── robots.txt
│   └── toggle-theme.js
├── src/
│   ├── assets/
│   │   └── socialIcons.ts
│   ├── components/
│   ├── content/
│   │   |  blog/
│   │   |    └── some-blog-post.md
│   │   └── config.ts
│   ├── layouts/
│   └── pages/
│   └── styles/
│   └── utils/
│   └── config.ts
│   └── types.ts
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its filename. 

Any static assets, like images, can be placed in the `public/` directory. All blog posts are stored in the `src/content/blog` directory.

## Commands

All command need to be run from the root of the project in a terminal:

> **_Note!_** For `Docker` commands you must have it [installed](https://docs.docker.com/engine/install/) before running any `docker` commands.

| Command                              | Relevant Action                                                                                                                  |
| :----------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| `npm install`                        | Installs dependencies                                                                                                            |
| `npm run dev`                        | Starts local dev server at `localhost:4321`                                                                                      |
| `npm run build`                      | Build your production site to `./dist/`                                                                                          |
| `npm run preview`                    | Preview your build locally, before deploying                                                                                     |
| `npm run format:check`               | Check code format with Prettier                                                                                                  |
| `npm run format`                     | Format with Prettier                                                                                                             |
| `npm run sync`                       | Generates TypeScript types for all Astro modules. [Learn more](https://docs.astro.build/en/reference/cli-reference/#astro-sync). |
| `docker compose up -d`               | Run AstroPaper on Docker, You can access with the same hostname and port informed using the `dev` command.                       |

> **_Warning!_** Windows PowerShell users may need to install the [concurrently package](https://www.npmjs.com/package/concurrently) if they want to [run diagnostics](https://docs.astro.build/en/reference/cli-reference/#astro-check) during development (`astro check --watch & astro dev`).

## Getting Started
- Clone this repository locally.
- Run these commands to build & run a development site to make your changes:
```
npm install
npm run build
npm run dev
```
- Alternatively, you can run this command to see how the live website will be served:
```
npm run preview
```
