# Personal Portfolio

A responsive personal portfolio website for **Warren Buffett Adrian**, built with Vue 3 and Vite. It introduces the developer, highlights skills and selected projects, shares a brief education and learning journey, and provides ways to get in touch.

## What’s included

- A home page with an introduction and portrait
- About, skills, projects, journey, and contact sections
- Responsive navigation with a mobile menu
- Dark and light themes, with the selected theme saved in the browser
- Project summaries for a personal finance tracker and a Sudoku solver
- Email, GitHub, and LinkedIn links

Portfolio content such as skills, project details, and journey entries is maintained in `src/data/portfolioData.js`. The page is assembled from Vue components in `src/components/`.

## Built with

- Vue 3
- Vite
- JavaScript and CSS

## Getting started

You’ll need Node.js and npm installed.

```sh
npm install
npm run dev
```

Vite prints the local development URL in the terminal.

## Available scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the local development server |
| `npm run build` | Create a production build in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run build:gh-pages` | Build with the GitHub Pages base path |
| `npm run deploy` | Build and publish `dist/` using `gh-pages` |
