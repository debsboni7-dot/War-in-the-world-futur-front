# Audit préliminaire des modèles 3D — Future Front

Date de l'audit : 2026-10-26

## Résultat

- 17 fichiers FBX repérés dans le dépôt.
- Taille totale des FBX : 81.55 MiB.
- Aucun fichier de texture séparé (`.png`, `.jpg`, `.webp`, etc.) n'apparaît dans l'arbre du dépôt au moment de l'audit.
- Cela ne prouve pas que les FBX n'ont pas de textures intégrées : le contenu binaire des FBX n'a pas été décodé ni inspecté visuellement.
- Aucun GLB optimisé n'a été trouvé dans l'arbre du dépôt.

## Armes (8)

- `Meshy_AI_Create_a_realistic_futuristic_rotary_20261025_generate.fbx` — 1.59 MiB
- `Meshy_AI_Realistic_futuristic_military_sniper_20261025_generate.fbx` — 1.59 MiB
- `Meshy_AI_Create_a_realistic_futuristic_pulse_20261025_generate.fbx` — 1.94 MiB
- `Meshy_AI_Realistic_futuristic_military_assault_20261025_generate.fbx` — 2.37 MiB
- `Meshy_AI_Realistic_futuristic_laser_rifle_with_20261025_generate.fbx` — 2.39 MiB
- `Meshy_AI_Realistic_futuristic_combat_shotgun_with_20261025_generate.fbx` — 2.68 MiB
- `Meshy_AI_Realistic_futuristic_heavy_machine_gun_20261025_generate.fbx` — 2.69 MiB
- `Meshy_AI_Realistic_futuristic_energy_pistol_for_a_20261025_generate.fbx` — 3.50 MiB

## Véhicules (6)

- `Meshy_AI_Create_a_realistic_futuristic_stealth_20261025_generate.fbx` — 2.50 MiB
- `Meshy_AI_Realistic_futuristic_compact_military_20261025_generate.fbx` — 3.26 MiB
- `Meshy_AI_Create_a_realistic_futuristic_heavy_20261025_generate.fbx` — 4.19 MiB
- `Meshy_AI_Create_a_compact_futuristic_military_20261025_generate.fbx` — 7.13 MiB
- `Meshy_AI_Create_a_realistic_futuristic_self_20261025_generate.fbx` — 12.99 MiB
- `Meshy_AI_Create_a_realistic_futuristic_amphibious_20261025_generate.fbx` — 18.16 MiB

## À identifier (3)

- `Meshy_AI_Create_a_realistic_futuristic_thermal_20261025_generate.fbx` — 2.37 MiB
- `Meshy_AI_Create_a_realistic_futuristic_20261025_generate.fbx` — 2.60 MiB
- `Meshy_AI_Create_a_realistic_futuristic_military_20261025_generate.fbx` — 9.60 MiB

## Ordre conseillé pour les tests

1. Commencer par le fichier d'arme le plus petit : `assets/models/weapons/Meshy_AI_Create_a_realistic_futuristic_rotary_20261025_generate.fbx` (1.59 MiB).
2. Vérifier le modèle dans un visualiseur 3D compatible FBX : géométrie, échelle, orientation, matériaux et textures.
3. Convertir en GLB avec textures incorporées si possible, puis mesurer le poids final et tester le chargement.
4. Tester ensuite le véhicule le plus petit : `assets/models/vehicles/Meshy_AI_Create_a_realistic_futuristic_stealth_20261025_generate.fbx` (2.50 MiB).
5. Ne pas charger les 17 modèles simultanément sur mobile. Charger uniquement le modèle requis pour la scène.

## État de validation

La présence et la taille des fichiers ont été vérifiées via l'arbre GitHub. Le contenu 3D lui-même reste à inspecter. Les catégories sont des hypothèses fondées sur les noms de fichiers, pas une validation visuelle.
