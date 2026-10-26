# Textures gratuites — War in the World: Future Front

## État actuel
- Le terrain utilise une texture de grain générée localement par Canvas (256×256, répétée sur la surface).
- Les bâtiments de l'avant-poste utilisent maintenant deux textures procédurales locales : béton marqué et métal peint strié.
- Ces textures sont générées au lancement, sans téléchargement ni licence tierce. Elles améliorent la variation de surface, mais ne sont pas des scans photoréalistes PBR.
- Les textures externes ci-dessous restent des sources vérifiées, mais elles ne sont **pas encore téléchargées ni intégrées** au dépôt.

## Sources avec licence vérifiée

1. **Poly Haven** — https://polyhaven.com/textures  
   Licence annoncée par la bibliothèque : CC0. Utilisation et redistribution autorisées sans attribution obligatoire. Licence : https://polyhaven.com/license
2. **ambientCG** — https://ambientcg.com/  
   Le site publie ses matériaux sous CC0. Vérifier la page et les fichiers de licence de chaque ressource avant de l'ajouter.
3. **Kenney — packs de textures** — https://kenney.nl/assets  
   Les pages de packs affichent la licence par pack; choisir uniquement ceux portant explicitement CC0. Détails : https://kenney.nl/support

## Matériaux à privilégier
- Sol principal : texture procédurale de terre/herbe.
- Avant-poste : textures procédurales de béton marqué et de métal strié.
- Prochaine étape : ajouter des cartes locales 1K de gravier/boue et améliorer les textures des arbres, une fois les fichiers externes téléchargés et leurs licences consignées.

## Profil mobile — Samsung Galaxy A06
- Commencer par des textures **1K (1024×1024)**; éviter de charger plusieurs ensembles 4K/8K.
- Utiliser une seule texture répétable pour les grandes surfaces.
- Charger les textures localement depuis le dépôt GitHub Pages, pas depuis des URL tierces au démarrage.
- Limiter le nombre de cartes PBR : base color + normal/roughness seulement si le rendu en a réellement besoin.
- Garder des textures compressées et surveiller la mémoire GPU; le poids total du dépôt affecte aussi le chargement mobile.

## Licence et attribution
CC0 signifie que l'attribution n'est pas obligatoire selon la déclaration des sources citées, mais conserver ce fichier de suivi aide à documenter la provenance. La licence de chaque asset précis doit être recontrôlée au moment du téléchargement.
