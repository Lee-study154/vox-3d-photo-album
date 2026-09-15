# VOX 手绘线稿 3D 相册

This local 3D photo album displays the supplied VOX PNGs through the
[`quick_flipbook`](https://github.com/bandinopla/quick_flipbook) page-turn engine.
The original files are copied byte for byte to `public/books/vox/` and are not edited.

The straight-on camera fits the open spread. The reader uses original-resolution
photo textures, contained within pages of differing aspect ratios, with page
curvature and soft lighting. No AI image generation or image editing is used.

```bash
npm ci
npm run dev
```

## Interaction

- Open the VOX edition from the library rail.
- Hover a page edge for a subtle lift, drag to scrub its turn, or click, swipe,
  and use the arrow keys.
- Home and End jump to the front and back covers.

## Verification

```bash
npm test
npm run build
```

## GitHub Pages

The repository includes a GitHub Actions workflow in
`.github/workflows/deploy-pages.yml`. Pushes to `main` run the tests, build the
static album, and publish `dist/` to GitHub Pages. Vite uses a relative asset
base so the album works at the repository's Pages subpath.

See [`THIRD_PARTY_NOTICES.md`](./THIRD_PARTY_NOTICES.md) for dependency attribution.

The source folder `/Users/liyuhan/Desktop/手绘线稿+VOX/成品/` remains untouched.
