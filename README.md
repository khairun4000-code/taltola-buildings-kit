# Taltola Khulna 3D - Building & House Kit (Code-Only, ~1.3 MB)

This lightweight kit contains the Three.js scene code (without heavy 3D car/character GLBs) so you can design and code new Bangladeshi houses & buildings compatible with the main game.

## Key Files
- src/house.js - 5-Story Taltola House (reference building with rooms, stairs, balconies, bathrooms)
- src/sk-arshan-tower.js - 10-Story Sk Arshan Alif Tower (modular helper makeB + interiors + elevator)
- src/scene-utils.js - Geometry helpers: box(), cylinder(), rodBetween(), mergeStaticMeshes()
- src/materials.js & src/aaa-shaders.js - Procedural PBR materials and textures
- src/khulna-geo.js - World coordinate system (1 unit = 1 meter, Y = up)
- src/khulna-corridors.js & src/khulna-landmarks.js - Street corridors & city landmarks

## How to Add a New Building
Export a function uildCustomBuilding(parent, m, offset = [0, 0, 0]) using ox(), cylinder(), 
odBetween(), and mergeStaticMeshes() so it can be dropped directly into 	altola-game.
