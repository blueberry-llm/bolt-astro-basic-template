# Astro Basic Template

A starter template for [bolt.diy](https://github.com/stackblitz-labs/bolt.diy).

## Purpose

This template is designed for use with **<https://github.com/stackblitz-labs/bolt.diy>**. bolt.diy fetches
these files at runtime and imports them into a fresh WebContainer project when you ask for an Astro project,
so everything here needs to install and build with no extra setup.

Modified by [Dustin Loring](https://github.com/Dustinwloring1988) (Dustinwloring1988) in October 2026.

## Stack

| Package | Version |
| --- | --- |
| Astro | ^7.3.8 |

## Commands

```bash
npm install   # install dependencies
npm run dev   # astro dev — dev server
npm run build # astro build — production build
npm run preview # astro preview — local preview server
```

## About this template

A minimal Astro project with a single `.astro` page. Astro's island architecture gives zero-JS HTML by
default. The build is handled by `astro build` and served by `astro preview`.

## Upgraded to Astro ^7.3.8 (October 2026)

The template originally had `astro` with a floating version. It was updated to `^7.3.8` (latest 7.x) to
ensure compatibility with the latest Astro tooling. `npm ci` was run fresh to install a clean dependency
tree, and `astro build` was verified to complete successfully. `astro check` reported 0 type errors.

Astro 7.x's build pipeline and Vite integration were confirmed working. No major version jump was needed
because Astro 8+ has different conventions (different config format, new directory structure) that would
require a larger migration beyond the scope of this update.

## Verification

- `npm ci && npm run build` passes with 0 errors
- `astro check` reports 0 errors
- `npm run preview` serves the production build correctly
- The generated HTML has no `id="__astro"` hydration markers (full static markup)