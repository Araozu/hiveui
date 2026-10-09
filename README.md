# Hive

Landing page for Hive, a control surface for AI agents running across the
machines you own. Built with Astro and Tailwind CSS v4.

## Commands

Run from the project root. Node and pnpm come from Vite+ (`vp`).

| Command          | Action                                      |
| :--------------- | :------------------------------------------ |
| `pnpm install`   | Install dependencies                        |
| `pnpm dev`       | Start the dev server at `localhost:4321`    |
| `pnpm build`     | Build the static site to `./dist/`          |
| `pnpm preview`   | Serve the production build locally          |

## Structure

```text
src/
  components/
    Comb.astro       hero honeycomb illustration (sessions as cells)
    HexMark.astro    placeholder logo; replace when the mark is designed
  layouts/
    Layout.astro     document head and global styles
  pages/
    index.astro      the one-page landing
  styles/
    global.css       Tailwind import, design tokens, grain, link style
public/
  favicon.svg        placeholder mark
```

## Design notes

- Tokens live in `src/styles/global.css` under `@theme`: six colours (wax,
  paper, propolis, honey, comb, resin) and two typefaces (Literata for display,
  Instrument Sans for text).
- Honey marks live work only. Hexagons are pointy-top, with flat sides left and
  right, in the logo and in the comb.
- The only motion is the hero load sequence. It is disabled under
  `prefers-reduced-motion`.
