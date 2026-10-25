# Shashank Singh | Portfolio

A dark, space-themed personal portfolio built with React, TypeScript and Tailwind CSS. It features a draggable WebGL project sphere in the hero, a looping space video background, an auto-moving projects carousel and a responsive tech stack section.


## Features

- **Interactive hero:** a draggable 3D sphere of project screenshots (React Bits `InfiniteMenu`, WebGL) that snaps the nearest project forward and shows its title and link.
- **Space video background:** a compressed looping video (about 1.6 MB, 720p) instead of a second WebGL scene, which keeps the page smooth.
- **Animated navigation:** an expandable card-style nav menu animated with GSAP.
- **Projects carousel:** an infinite, auto-moving carousel with mouse drag, momentum, mouse-wheel scrolling, pause on hover and arrow controls. It is built without a carousel library.
- **Tech stack section:** categorised cards with icons and scroll-reveal animations (AOS), fully responsive from mobile to desktop.
- **About and footer:** short intro, academic and experience highlights, and contact links (GitHub, LinkedIn, Email).

## Tech Stack

| Area | Tools |
| --- | --- |
| Framework | React 19, TypeScript, Vite |
| Styling | Tailwind CSS 4, tw-animate-css |
| Animation | GSAP, AOS |
| 3D and WebGL | Three.js, React Three Fiber, OGL, gl-matrix |
| Icons | React Icons, Lucide |
| Deployment | GitHub Pages (GitHub Actions) |

## Project Structure

```
portfolio-website/
├── public/                 # Static assets (project screenshots, space video, favicon)
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── About.tsx
│   │   ├── BackGround.tsx
│   │   ├── CardNav.tsx        # Expandable navigation
│   │   ├── Cards.tsx          # Academic and experience highlights
│   │   ├── Footer.tsx
│   │   ├── InfiniteMenu.tsx   # WebGL project sphere
│   │   ├── Projects.tsx       # Auto-moving carousel
│   │   └── TechStack.tsx
│   ├── App.tsx
│   ├── App.css
│   ├── index.css
│   └── main.tsx
├── index.html
├── vite.config.ts
└── package.json
```

## Deployment

The site is deployed to GitHub Pages. Pushing to the main branch triggers the build workflow, and the site updates in a minute or two.

If the site is served from a sub-path (`username.github.io/repo-name/`), set the base path in `vite.config.ts`:

```ts
export default defineConfig({
  base: "/repo-name/",
  // ...
});
```

## Acknowledgements

- [React Bits](https://reactbits.dev) for the `InfiniteMenu` and `CardNav` components.
- [AOS](https://michalsnik.github.io/aos/) for scroll animations.

## Contact

**Shashank Singh**
- GitHub: [@shashank-bingading](https://github.com/shashank-bingading)
- LinkedIn: https://www.linkedin.com/in/shashanksingh88
- Email: shashanksinghwork88@gmail.com
