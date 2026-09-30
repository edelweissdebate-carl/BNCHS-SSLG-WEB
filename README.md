# BNCHS SSLG Information Hub v5

This build contains **53 official BNCHS SSLG Facebook posts/reels** supplied for the archive, starting with Committee Induction Day and ending at the September 30, 2026 cutoff.

## What changed in v5
- Every story card uses the **real cover/poster/reel thumbnail from the official post**.
- No generated green/blue title-card covers are used.
- Every article contains an **At-a-glance / complete published details** panel plus a self-contained article.
- Original Facebook links remain at the bottom only as sources.
- The Committee Induction post includes an official multi-photo gallery.

## Why the hosted version has `/api/cover.js`
Facebook image-CDN links are signed and expire. The current cover URLs work in the standalone HTML for immediate testing, but they are not permanent. When hosted on Vercel, the site uses `/api/cover.js` to read a fresh `og:image` from the exact official post and proxy it to the page. If that refresh ever fails, the browser tries the current direct cover URL as a fallback.

## Recommended deployment + Google Sites
1. Upload this whole folder to a GitHub repository or directly to Vercel.
2. Deploy it on Vercel.
3. Open your Google Site.
4. Insert → Embed → By URL.
5. Paste the Vercel site URL and resize the embed.

The standalone HTML is for local preview. The Vercel-ready folder/ZIP is the recommended permanent version because it can refresh Facebook cover URLs.
