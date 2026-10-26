# Tester une arme FBX directement depuis Android

Le jeu utilise maintenant le chargeur Three.js `FBXLoader` et tente de charger le FBX déjà présent dans le dépôt : `assets/models/weapons/Meshy_AI_Create_a_realistic_futuristic_rotary_20261025_generate.fbx` (environ 1,59 Mio).

## Ce qui se passe en jeu

- Le chargeur demande uniquement cette arme légère au démarrage.
- Les 16 autres FBX ne sont pas chargés.
- L'arme provisoire reste visible si le module FBXLoader ou le fichier FBX échoue à charger.
- En cas de chargement réussi, le code normalise la taille approximative du modèle et remplace l'arme provisoire.

## Test à effectuer sur Android

1. Ouvre le jeu via GitHub Pages après la publication du dernier commit.
2. Recharge la page avec une connexion internet active (Three.js et FBXLoader viennent d'un CDN).
3. Regarde si le modèle apparaît dans la main du personnage et vérifie les FPS.
4. Si l'arme est invisible, trop grande, tournée dans le mauvais sens ou sans textures, le FBX peut nécessiter un ajustement supplémentaire. La normalisation actuelle ne peut pas deviner automatiquement l'orientation correcte.

## Limites connues

- Le FBX fait environ 1,59 Mio, mais il peut contenir des matériaux ou des données supplémentaires qui affectent le temps de chargement.
- Les textures externes éventuelles doivent être accessibles par des chemins compatibles ; la présence de fichiers de textures séparés n'a pas été confirmée.
- Le changement de code n'a pas encore été testé dans un navigateur réel. Ne considère pas l'arme comme validée avant un test sur l'appareil.
