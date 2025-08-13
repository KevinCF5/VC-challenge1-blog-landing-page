## VC Challenge 1 — Blog Landing Page

A pixel-focused implementation of a blog landing page based on a community Figma. The page showcases a hero banner, a galleries strip, and a grid of featured articles, ending with a footer. Built with semantic HTML and modern, utility-style CSS without any JavaScript.

### Figma

- Design reference: [Viver de Código — Desafio 1](https://www.figma.com/design/JNpSqGAx3mQb5PDMlmX849/Viver-de-Código---Desafio--1---21-04-a-27-04?t=uwexw2KpqqDyuLVb-1)

<img width="365" height="845" alt="image" src="https://github.com/user-attachments/assets/2749e6be-57f8-48ba-94d5-47a750309703" />

### Preview / Screenshots

![Hero (desktop)](assets/images/screenshots/hero-desktop.png)
![Articles grid (desktop)](assets/images/screenshots/articles-desktop.png)
![Footer (desktop)](assets/images/screenshots/footer-desktop.png)

### Tech Stack

- **HTML5**: semantic structure (`header`, `main`, `section`, `article`, `footer`, `nav`).
- **CSS3**: custom properties, gradients, Flexbox, CSS Grid, absolute positioning for decorative assets.
- **Google Fonts**: Fira Sans Condensed, Inter, Quicksand.

### Techniques Used

- **CSS Custom Properties**: centralized theme in `assets/css/_variables.css` (colors, weights, gradients).
- **Gradient text** using `background-clip: text` for the hero headline.
- **Radial gradient highlights** via pseudo-elements to create soft glows behind artwork.
- **Layout systems**: Flexbox for alignment and CSS Grid for the articles section (`grid-column` spans, fixed and flexible tracks).
- **Layered imagery**: absolute positioning, `z-index`, and responsive containment using the `.container` max-width pattern.
- **Typography scale** with rems and consistent font weights.

### What I Focused On

- Translating the Figma spacing and color system into reusable CSS variables.
- Building clean, readable markup with clear class responsibilities.
- Achieving visual hierarchy through weight, size, and color contrasts.

### Challenges & How I Solved Them

- **Layering and overlap of images**: Managing stacking contexts and precise offsets for overlapping cards and avatars using `position: absolute` and careful `z-index` ordering.
- **Gradient text legibility**: Ensuring cross-browser consistency with `-webkit-text-fill-color: transparent` in addition to `background-clip`.
- **Grid spanning and alignment**: Getting the two-row articles layout to align with mixed content sizes by combining fixed track sizes with `grid-column` spans.
- **Consistency with Figma spacing**: Standardized to rems and applied shared spacing via utility-like class patterns in CSS.

### Project Structure

```
VC-challenge1-blog-landing-page/
  index.html
  assets/
    css/
      _variables.css
      main.css
    images/
    screenshots/
```

### Project Links

Github: https://github.com/KevinCF5/VC-challenge1-blog-landing-page
Blog Page: https://vc-challenge1-blog-landing-page.vercel.app/

### Improvements to Explore

- Add responsive breakpoints for tablet/mobile.
- Improve Gallery section by adjusting the width of the container.
- Implement minimal JS for navigation interactions if needed.

### Acknowledgements

- Design challenge by Viver de Código.
