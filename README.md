# Scentique 🌸

A modern, fully responsive single-page landing website for a luxury perfume brand. Built with pure HTML and CSS — no frameworks, no JavaScript, no build tools.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Font Awesome](https://img.shields.io/badge/Font_Awesome-528DD7?style=flat&logo=fontawesome&logoColor=white)

---

## What It Does

Scentique is a polished e-commerce-style landing page for a fictional luxury fragrance brand. It showcases a full product experience across ten thematic sections — from a full-viewport hero to a pricing table, testimonials, and a team showcase — all styled with a cohesive coral/salmon colour palette and smooth CSS hover transitions.

## Features

- **10 richly styled sections**: Hero, Features, Signature Collection, Services, About, Stats, Pricing, Testimonials, Team, and News
- **Fixed navigation header** with a search bar and a hover-triggered dropdown menu
- **Parallax-style backgrounds** using `background-attachment: fixed` on the stats and testimonials sections
- **CSS-only hover effects** — card fills, image overlays, link underline animations, and opacity transitions
- **Self-hosted Font Awesome** — no CDN dependency at runtime for icons
- **Optimised images** — all images use the modern `.avif` format for smaller file sizes
- **Google Fonts integration** — uses the _Nunito_ typeface for a clean, rounded look
- **Zero JavaScript** — every interaction is achieved with pure CSS

## Project Structure

```
scentique/
├── index.html          # Single-page markup (all 10 sections)
├── css/
│   ├── style.css       # All custom styles, organised by section
│   └── all.css         # Self-hosted Font Awesome stylesheet
├── images/             # AVIF images for backgrounds and cards
│   ├── section-1-bg.avif
│   ├── s3-img1.avif … s3-img6.avif
│   └── …
└── webfonts/           # Font Awesome font files (ttf + woff2)
```

## Getting Started

No installation or build step is required.

### Prerequisites

Any modern web browser (Chrome, Firefox, Safari, Edge).

### Running locally

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/scentique.git
   cd scentique
   ```

2. **Open in a browser**

   Simply open `index.html` directly:

   ```bash
   # macOS
   open index.html

   # Linux
   xdg-open index.html

   # Windows
   start index.html
   ```

   Or drag the file into any browser window — no local server is needed.

> **Tip:** For the best experience (and to avoid any browser security restrictions on local fonts/images), you can serve the project with a simple local server:
>
> ```bash
> # Python 3
> python -m http.server 8080
>
> # Node.js (npx)
> npx serve .
> ```
>
> Then visit `http://localhost:8080`.

## Page Sections

| #   | Section                  | Description                                                                       |
| --- | ------------------------ | --------------------------------------------------------------------------------- |
| 1   | **Hero**                 | Full-viewport background image with CTA buttons                                   |
| 2   | **Welcome**              | Three feature cards (Personalised Fragrance, Signature Scents, Online Experience) |
| 3   | **Signature Collection** | Six product images with hover overlay revealing name and actions                  |
| 4   | **What We Offer**        | Six service cards (Luxury Brands, Exclusive Editions, Easy Shopping, …)           |
| 5   | **Why Choose Scentique** | Left-aligned text with key selling points alongside a portrait image              |
| 6   | **Stats**                | Parallax banner — 451k clients, 15 awards, 154k coffees, 45 projects              |
| 7   | **Pricing**              | Cards for Dior Sauvage ($95), Chanel No. 5 ($130), Tom Ford Noir ($120)           |
| 8   | **Testimonials**         | Parallax banner with two customer quotes                                          |
| 9   | **Team**                 | Cards for Ahmed, Omar, and Hassan with social icon links                          |
| 10  | **News**                 | Three blog-style cards with author, date, and a read-more link                    |

## Customisation

All colours, spacing, and typography are controlled in `css/style.css`. The primary brand colour is defined inline throughout the file as:

```css
rgb(240, 117, 117)   /* coral / salmon pink */
```

To retheme the site, do a find-and-replace on that value in `css/style.css`.

Fonts are loaded from Google Fonts in `index.html`. To change the typeface, swap the `<link>` tag in the `<head>` and update the `font-family` declaration in the `body` rule inside `css/style.css`.

## Browser Support

Works in all evergreen browsers. `background-attachment: fixed` (used for parallax) is not supported on iOS Safari — those sections will display a static background instead.

## Contributing

1. Fork the repository and create a feature branch (`git checkout -b feature/my-change`)
2. Make your changes to `index.html` or `css/style.css`
3. Test in at least two browsers
4. Open a pull request with a clear description of what you changed and why

Please keep pull requests focused — one feature or fix per PR.

## License

This project is released for educational and personal-portfolio use. All images are project-specific assets — please replace them with properly licensed images before any commercial use.
