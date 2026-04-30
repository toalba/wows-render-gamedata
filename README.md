# wows-render-gamedata

Curated subset of World of Warships game data, used by [wows-renderer](https://github.com/toalba/wows-renderer) and [wows-replay-parser](https://github.com/toalba/wows-replay-parser).

This repo is generated automatically from the game client. Every WoWs build that produces an entry here is tagged `v<build_id>`.

## Layout

```
data/
├── content/GameParams.data    Binary entity database
├── gui/                       Renderer-required icon/silhouette assets
├── spaces/                    Minimap PNGs and space.settings
├── scripts_entity/            Entity .def schemas + alias.xml
├── global.mo                  GNU gettext localization
└── *.json                     Curated lookup tables (ships, projectiles, …)
```

## Tags

Tags follow the pattern `v<build_id>` where the build ID is the WoWs client build (e.g. `v12267945`). `wows-replay-parser` uses these tags to fetch matching data for a given replay.

## License

Repository scaffolding is provided under the Apache License 2.0 — see [LICENSE](LICENSE).

World of Warships game assets republished here (icons, maps, GameParams binary, localization, entity schemas) remain the copyright of Wargaming. See [NOTICE](NOTICE) for attribution.
