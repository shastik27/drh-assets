# Dead Road Heroes — game-ready art pack (v1)

- `atlas/characters.png|json` — hero (4 evolution stages), 6 enemies, pickups. Phaser 3 "JSON Hash" atlas.
- `atlas/world.png|json` — path tiles, node pad, walls, stairs, props.
- `sprites/*.png` — the same images as separate files (transparent PNG).
- `ground/*_seamless.png` — tileable ground textures (grass, dirt, asphalt) for TileSprite backgrounds.
- `assets-manifest.json` — size, anchor (origin), footprint in tiles, description of every sprite + iso grid formula.
- `preview_scene.jpg` — static mockup showing intended scale and composition.

Isometric grid: tileWidth 256, tileHeight 162 (diamond).  
screenX = (col - row) * 128, screenY = (col + row) * 81. Draw back-to-front by screenY.  
Use `setOrigin(anchor[0], anchor[1])` from the manifest for every sprite.
