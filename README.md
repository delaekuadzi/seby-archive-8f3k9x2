# SebyGames Retro Archive

Static Flash game archive for SebyGames Retro, served through GitHub + jsDelivr and played through Ruffle on the main SebyGames site.

## Structure

```text
games/cartoon-network/<game-slug>/game.swf
games/cartoon-network/<game-slug>/assets/
games/disney/<game-slug>/game.swf
games/nickelodeon/<game-slug>/game.swf
games/other/<game-slug>/game.swf
```

## Counts

- cartoon-network: 35
- other: 40

## CDN URL Pattern

```text
https://cdn.jsdelivr.net/gh/delaekuadzi/seby-archive-8f3k9x2@main/games/<category>/<game-slug>/game.swf
```

## Notes

- Do not upload launchers, installers, executables, torrents, caches, or source archives.
- Keep `games.json` schema stable; SebyGames imports it for Ruffle playback.
- Reports live in `reports/`.
