# Uber Partners Landing Page

A responsive marketing landing page for an **Uber partner in Moscow**. It is aimed at drivers who want to join the service with their own car or a company vehicle.

This is a front-end project. It is **not** an official Uber product.

## What the page includes

- Header with navigation, partner branding, and a call-back request
- Promo block inviting drivers to apply
- Eight reasons to work with the partner (cashless payments, commission, flexible hours, support, and more)
- Uber mobile app highlights
- Driver requirements (own car vs company car)
- Cities / worldwide coverage section
- Footer with contacts and store badges
- Hamburger menu for smaller screens

Page copy is in **Russian**.

## Tech stack

| Area | Tools |
| --- | --- |
| Markup | HTML5 |
| Layout | Bootstrap Grid & Reboot |
| Styles | Sass, Autoprefixer, CleanCSS |
| Scripts | vanilla JavaScript |
| Icons / fonts | Font Awesome, Google Fonts (Roboto) |
| Build | Gulp 4 |
| Dev server | BrowserSync |

## Project structure

```
src/                 source files
  index.html
  sass/              styles (variables, mixins, layout, media queries)
  js/script.js       mobile menu toggle
  css/               vendor CSS (Bootstrap)
  icons/  img/       assets
dist/                build output (served by BrowserSync)
gulpfile.js          compile, minify, copy, watch, live reload
```

Gulp compiles Sass to minified CSS, minifies HTML, and copies scripts, fonts, icons, and images into `dist/`.

## Getting started

**Requirements:** Node.js and npm.

```bash
npm install
npx gulp
```

This starts the default Gulp task: build into `dist/`, watch `src/` for changes, and open a local BrowserSync server.

Open the URL shown in the terminal (usually `http://localhost:3000`).

## Scripts

There is no `npm start` script. Use Gulp directly:

| Command | Description |
| --- | --- |
| `npx gulp` | Build, watch, and serve `dist/` |
| `npx gulp styles` | Compile and minify Sass only |
| `npx gulp html` | Minify HTML into `dist/` |

