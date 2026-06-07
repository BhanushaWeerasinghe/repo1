# Hotel Website — Static Template (HTML, CSS, JavaScript)

A clean, responsive hotel/restaurant website template built with plain HTML, CSS (Sass source included), and JavaScript. This repository contains the full static site sources and assets (images, fonts, CSS, JS) so you can run it locally, customize it, or deploy to a static hosting provider like GitHub Pages or Netlify.

![preview image](/preview.png)

## Table of Contents

- [Features](#features)
- [Live Preview](#live-preview)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Development & Customization](#development--customization)
- [Deploying](#deploying)
- [Assets & Licenses](#assets--licenses)
- [Contributing](#contributing)
- [Author / Contact](#author--contact)
- [License](#license)

## Features

- Responsive layout for hotel/restaurant pages
- Multiple HTML pages: home, about, rooms, restaurant menu, blog, contact
- Sass source files under `scss/` for easy theming and rebuilds
- Common UI components: navigation, hero sections, galleries, carousels, date picker
- Lightweight vanilla JavaScript for interactive widgets (carousel, maps stub, modal popups)

## Live Preview

If you enable GitHub Pages for this repository (or deploy to another static host) you'll be able to preview the site live. Example URL (replace with your username and repository):

`https://<your-github-username>.github.io/repo1/`

## Getting Started

Prerequisites:

- A modern web browser
- (Optional) Node.js + npm if you want to compile Sass or run a dev server

Quick local preview (no build tools required):

PowerShell (works on Windows):

```powershell
# Start a simple static server using Python (if Python is installed):
python -m http.server 8000

# Or, using an npm-based static server (if Node.js is installed):
npx http-server -c-1 . -p 8000
```

Then open http://localhost:8000 in your browser.

Notes:

- If you don't have Python/Node available, opening `index.html` directly in the browser works for static content, but some features (AJAX, maps) may require a server.

## Project Structure

Top-level files and directories:

- `index.html` — Home / landing page
- `about.html` — About page
- `rooms.html`, `rooms-single.html` — Rooms listing and detail
- `restaurant.html` — Menu / restaurant page
- `blog.html`, `blog-single.html` — Blog listing and article
- `contact.html` — Contact page (form UI only)
- `css/` — Compiled CSS and vendor styles
- `scss/` — Sass source files for styling (edit & recompile if you change variables)
- `js/` — JavaScript files and vendor libraries
- `images/` — Site images and assets
- `fonts/` — Font files used by the theme
- `readme.md` — This file

## Development & Customization

- To change styles, edit the files in `scss/` and recompile to `css/style.css`. If you have `sass` installed:

```powershell
# install sass if needed
npm install -g sass
# compile once
sass scss/style.scss:css/style.css --style=expanded
# or watch for changes
sass --watch scss:css
```

- JavaScript is mostly vanilla; you can replace or update files under `js/`. Vendor libs (jQuery, Owl Carousel, AOS) are included in `js/` and `css/`.
- Replace images in `images/` but keep the same filenames if you want to avoid updating HTML references.

## Deploying

GitHub Pages (recommended for static sites):

1. Push the repository to GitHub (already done for this repo).
2. In the repository Settings → Pages, select branch `main` and folder `/ (root)` and click Save.
3. After a minute, your site will be available at `https://<your-github-username>.github.io/repo1/`.

Other hosts: Netlify, Vercel, Surge, or any static web host accept the same build output.

## Assets & Licenses

- Fonts and images included in `fonts/`, `images/`, and `flaticon/` may be subject to their original licenses. Check the vendor license files inside the font folders (for example `fonts/flaticon/license/`) before using the assets commercially.
- Third-party libraries bundled in `js/` and `css/` (Bootstrap, jQuery, Owl Carousel, AOS, etc.) are generally open-source but follow their respective licenses. See vendor documentation for details.

## Contributing

If you want to contribute improvements:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-change`
3. Make changes and commit: `git commit -am "Add my change"`
4. Push and open a Pull Request

Small improvements I can help with on request:

- Add a `.gitignore`
- Add a proper `LICENSE` file
- Convert local JS/CSS includes to CDN-based includes for smaller repo size

## Author / Contact

Repository: https://github.com/BhanushaWeerasinghe/repo1

If you'd like further help customizing the template, tell me what to change (colors, layout, or add pages) and I can make the edits.

## License

This repository does not include a license file. If you want to open-source it, add a `LICENSE` (for example MIT) or tell me which license to apply and I can add it for you.