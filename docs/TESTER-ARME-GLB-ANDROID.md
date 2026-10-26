# Tester une arme GLB depuis Android

Le jeu peut maintenant charger facultativement `assets/models/weapons/rotary.glb`. Si le fichier n'existe pas, ou si le chargement échoue, le jeu conserve son arme provisoire légère : le démarrage ne dépend donc pas de ce modèle.

## Étapes sur téléphone

1. Ouvre le dépôt GitHub : https://github.com/debsboni7-dot/War-in-the-world-futur-front
2. Dans `assets/models/weapons/`, télécharge le FBX `Meshy_AI_Create_a_realistic_futuristic_rotary_20261025_generate.fbx` (environ 1,59 Mio).
3. Ouvre le convertisseur dans Chrome : https://poyo.ai/free-tools/fbx-to-glb
4. Choisis le FBX téléchargé, vérifie que le modèle apparaît correctement, puis exporte en GLB.
5. Dans GitHub sur Android, ouvre `assets/models/weapons/` et utilise l'option d'ajout de fichier pour téléverser le GLB converti. Nomme-le exactement `rotary.glb`.
6. Attends que GitHub Pages publie le commit, puis recharge le jeu. Teste le modèle et les FPS.

## Vérifications importantes

- Le convertisseur annonce un traitement dans le navigateur, sans téléversement du FBX.
- La conversion ne garantit pas que l'orientation, l'échelle, les matériaux ou les textures seront parfaits. Vérifie l'aperçu avant d'exporter.
- Sur le téléphone, un modèle qui charge mais paraît trop grand, orienté de travers ou sans texture doit être corrigé avant de l'utiliser en jeu.
- Le chargeur du jeu masque l'arme provisoire uniquement après un chargement GLB réussi. En cas d'échec, le prototype conserve l'arme provisoire.
- Le GLB n'est pas encore inclus dans le dépôt. Il faut effectuer les étapes ci-dessus pour tester le vrai modèle.
