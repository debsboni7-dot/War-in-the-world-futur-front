# Textures gratuites — War in the World: Future Front

## État actuel
- Le terrain de `index.html` utilise désormais une texture de bruit générée par Canvas à l'exécution (256×256, répétée). Elle ne télécharge aucun fichier externe et n'a pas de licence tierce.
- Cette modification est un premier traitement visuel léger, pas un pack de textures photoréalistes.
- Les textures externes ci-dessous sont des sources vérifiées, mais elles ne sont **pas encore téléchargées ni intégrées** au dépôt.

## Sources avec licence vérifiée

1. **Poly Haven** — https://polyhaven.com/textures  
   Licence annoncée par la bibliothèque : CC0. Utilisation et redistribution autorisées sans attribution obligatoire. Licence : https://polyhaven.com/license
2. **ambientCG** — https://ambientcg.com/  
   Le site publie ses matériaux sous CC0. Vérifier la page et les fichiers de licence de chaque ressource avant de l'ajouter.
3. **Kenney — packs de textures** — https://kenney.nl/assets  
   Les pages de packs affichent la licence par pack; choisir uniquement ceux portant explicitement CC0. Détails : https://kenney.nl/support

## Matériaux à privilégier
- Sol principal : terre/herbe ou terrain poussiéreux.
- Zones de combat : gravier, boue et béton.
- Avant-poste : béton usé et métal peint/griffé.

## Profil mobile — Samsung Galaxy A06
- Commencer par des textures **1K (1024×1024)**; éviter de charger plusieurs ensembles 4K/8K.
- Utiliser une seule texture répétable pour les grandes surfaces.
- Charger les textures localement depuis le dépôt GitHub Pages, pas depuis des URL tierces au démarrage.
- Limiter le nombre de cartes PBR : base color + normal/roughness seulement si le rendu en a réellement besoin.
- Garder des textures compressées et surveiller la mémoire GPU; le poids total du dépôt affecte aussi le chargement mobile.

## Licence et attribution
CC0 signifie que l'attribution n'est pas obligatoire selon la déclaration des sources citées, mais conserver ce fichier de suivi aide à documenter la provenance. La licence de chaque asset précis doit être recontrôlée au moment du téléchargement.
