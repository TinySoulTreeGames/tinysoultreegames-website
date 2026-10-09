# Tiny Soul Tree Games

Official studio website. A small coming-soon page for Soul Crossing and future games, with a celestial Soul Tree banner and under-construction details.

## Put it online with Cloudflare Pages

1. In Cloudflare, open **Workers & Pages → Create application → Pages → Import an existing Git repository**.
2. Connect GitHub and select **TinySoulTreeGames/tinysoultreegames-website**.
3. Use these settings:

| Setting | Value |
| --- | --- |
| Production branch | `main` |
| Framework preset | None |
| Build command | `exit 0` |
| Build output directory | `public` |
| Root directory | Leave unchanged / repository root |

4. Deploy. Cloudflare supplies a `pages.dev` URL. Add your domain using the project's **Custom domains** section when ready.

No package install, environment variables, database or API keys are required. This is a static HTML/CSS site. Publishing `public` keeps project notes outside the hosted website.

[Cloudflare's static HTML guide](https://developers.cloudflare.com/pages/framework-guides/deploy-anything/)

## Edit and preview

- `public/index.html`: text and social link.
- `public/styles.css`: desktop/mobile layout and colors.
- `public/assets/soul-tree-banner.webp`: original atmospheric studio illustration, not gameplay footage.
- `public/assets/spark.svg`: small decorative favicon, not a replacement for the studio's official logo.

Preview with `python -m http.server 4173 --directory public`, then open `http://localhost:4173`.

The page includes no analytics, tracking, cookies, forms or external font dependencies. The X link opens the account supplied by the owner. Once a final domain is connected, set `og:image` to its absolute banner URL and add the canonical/og:url metadata for reliable social sharing.

Banner generated with the built-in Imagegen tool. Editable page text is HTML rather than part of the image. See `ASSET-NOTES.md` for the image brief.
