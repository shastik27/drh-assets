# Dead Road Heroes — game-ready art pack (v1)

- `atlas/characters_v2.png|json` — hero (4 stages), 13 enemies, 4 survivors, pickups (key, hammer, crystal, dig spot). (v1 atlases kept for old builds)
- `atlas/world_v2.png|json` — path tiles, node pad, portals, gates, bridge, one-way tile, toxic trap, chest, walls, props.
- `badges/*.png` — 16 round 160px icon badges for mechanics and UI.
- `sprites/*.png` — the same images as separate files (transparent PNG).
- `ground/*_seamless_v2.png` — tileable ground textures (grass, dirt, asphalt) for TileSprite backgrounds.
- `assets-manifest.json` — size, anchor (origin), footprint in tiles, description of every sprite + iso grid formula.
- `preview_scene.jpg` — static mockup showing intended scale and composition.

Isometric grid: tileWidth 256, tileHeight 162 (diamond).  
screenX = (col - row) * 128, screenY = (col + row) * 81. Draw back-to-front by screenY.  
Use `setOrigin(anchor[0], anchor[1])` from the manifest for every sprite.
