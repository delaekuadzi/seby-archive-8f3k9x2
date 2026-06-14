# Future Cloudflare R2 Migration Plan

The GitHub/jsDelivr archive intentionally mirrors the future R2 object layout.

## Current CDN Base

`https://cdn.jsdelivr.net/gh/delaekuadzi/seby-archive-8f3k9x2@main`

## Future R2 Base

`https://retro.sebygames.com`

## Migration Steps

1. Upload the `games/` directory to the R2 bucket root without changing object keys.
2. Replace the manifest CDN base from `https://cdn.jsdelivr.net/gh/delaekuadzi/seby-archive-8f3k9x2@main` to `https://retro.sebygames.com`.
3. Keep per-game paths unchanged, for example:
   - `games/cartoon-network/<slug>/game.swf`
   - `games/other/<slug>/game.swf`
4. Configure immutable cache headers for uploaded objects.
5. Keep `games.json` in SebyGames synchronized with the new base URL.
6. Validate a representative sample from each category through Ruffle.

## Current Archive Size

- Games: 75
- Categories: other, cartoon-network
