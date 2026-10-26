# Asset pipeline — Future Front

## Folder map
- `assets/models/` — 3D models (GLB recommended)
- `assets/textures/` — textures and material maps
- `assets/vfx/` — visual effects and effect textures
- `assets/audio/` — sound effects, ambience, music
- `assets/animations/` — animation resources and notes
- `assets/ui/` — interface graphics
- `assets/fonts/` — fonts and licenses
- `assets/data/` — JSON data for weapons, missions, enemies, and items

## Adding an asset
1. Upload it to the matching folder using GitHub's **Add file → Upload files** on your phone.
2. Give files clear, lowercase names with hyphens, e.g. `scout-rifle.glb`.
3. Keep related files together and add a README or source/license note when needed.
4. Reference assets in game code with repository-relative paths, e.g. `assets/models/weapons/scout-rifle.glb`.
5. Test the game after adding assets. Large binary files increase download time and may hurt mobile performance.

## Important
GitHub's web editor is best for small text files. For binary assets (GLB, PNG, WebP, audio), use **Add file → Upload files**. Do not upload API keys or private credentials.
