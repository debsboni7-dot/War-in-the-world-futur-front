# Textures gratuites — War in the World: Future Front

## État actuel
- Le terrain utilise une texture de grain générée localement par Canvas (256×256, répétée sur la surface).
- Les bâtiments de l'avant-poste utilisent deux textures procédurales locales : béton marqué et métal peint strié.
- Les troncs ont maintenant un grain vertical dédié; les feuillages utilisent des marques ovales façon feuilles, générées localement. La grille de débogage visible au sol a été retirée pour garder un terrain continu.
- Ces textures sont générées au lancement, sans téléchargement ni licence tierce. Elles améliorent la variation de surface, mais ne sont pas des scans photoréalistes PBR.
- Le jeu tente maintenant de charger trois cartes photographiques 1K depuis les URL directes de Poly Haven : gravier/béton pour le terrain, béton pour les bâtiments et métal peint rouillé pour les toits. Elles sont chargées à l'exécution; elles ne sont pas copiées dans le dépôt. Si une URL ou la connexion échoue, les textures procédurales restent en place.

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
- Végétation : textures procédurales d'écorce et de feuillage.
- Cartes photographiques chargées : `gravel_embedded_concrete_diff_1k.jpg`, `concrete_floor_diff_1k.jpg` et `rusty_painted_metal_diff_1k.jpg` (Poly Haven, CC0). Le chargement à distance nécessite une connexion internet; pour un chargement hors ligne fiable, il faudra ensuite empaqueter ces fichiers dans le dépôt.

## Profil mobile — Samsung Galaxy A06
- Commencer par des textures **1K (1024×1024)**; éviter de charger plusieurs ensembles 4K/8K.
- Utiliser une seule texture répétable pour les grandes surfaces.
- Charger les textures localement depuis le dépôt GitHub Pages, pas depuis des URL tierces au démarrage.
- Limiter le nombre de cartes PBR : base color + normal/roughness seulement si le rendu en a réellement besoin.
- Garder des textures compressées et surveiller la mémoire GPU; le poids total du dépôt affecte aussi le chargement mobile.

## Licence et attribution
CC0 signifie que l'attribution n'est pas obligatoire selon la déclaration des sources citées, mais conserver ce fichier de suivi aide à documenter la provenance. La licence de chaque asset précis doit être recontrôlée au moment du téléchargement.
