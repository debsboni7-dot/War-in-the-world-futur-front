# Audit et texturation des modèles 3D — Future Front

## Outil de contrôle sur mobile
Page : `model-preview.html` (GitHub Pages). Elle charge un seul modèle à la fois et affiche :
- le nombre de mailles et de matériaux ;
- les matériaux qui ont déjà une image de texture ;
- les matériaux sans image ;
- la présence d'UV ;
- une texture procédurale de secours à l'écran pour les matériaux sans image.

## Fallback déjà ajouté au jeu
Le modèle FBX de l'arme rotative chargé par `index.html` reçoit maintenant la texture procédurale métallique du jeu si ses matériaux n'ont pas de texture image. C'est un fallback visuel à l'exécution, pas une modification du FBX d'origine.

## Limites importantes
- Le fichier FBX source n'est pas modifié et aucun fichier de texture n'a été incorporé/exporté dans les modèles.
- La texture de secours ne remplace pas une vraie texture PBR : elle sert à éviter un matériau entièrement plat et à faciliter l'inspection.
- Les textures potentiellement intégrées aux FBX/GLB doivent être vérifiées dans la page d'inspection. Le nombre de matériaux avec image ne prouve pas à lui seul que la texture est correctement UV-mappée ou visuellement correcte.
- Les FBX doivent être contrôlés individuellement, puis convertis en GLB optimisés avant d'être ajoutés au gameplay. Ne pas charger tous les modèles en même temps sur le téléphone.
- Les modèles rangés dans `robots` et `structures` sont classés d'après leur nom de fichier ; leur type exact doit encore être confirmé visuellement.

## Procédure de validation
1. Ouvrir la page d'inspection après la mise à jour GitHub Pages.
2. Choisir un modèle et appuyer sur « Charger / analyser ».
3. Faire pivoter le modèle en glissant dans la zone de visualisation.
4. Noter le nombre de matériaux sans image et vérifier l'aspect des textures.
5. Prioriser les petits modèles (armes) ; tester les véhicules ensuite.
6. N'intégrer dans le jeu que les modèles vérifiés, convertis en GLB et optimisés.

## État actuel
- [x] Répartition des modèles dans les dossiers du dépôt.
- [x] Création d'une page d'inspection mobile avec rapports matériaux/UV.
- [x] Texture procédurale de secours dans l'aperçu.
- [x] Texture métallique de secours dans le jeu pour l'arme FBX actuellement chargée si elle n'a pas de map.
- [ ] Inspection visuelle de chaque modèle sur l'appareil.
- [ ] Textures PBR finales incorporées dans les modèles.
- [ ] Conversion et optimisation de chaque modèle FBX en GLB.
- [ ] Tests de performance sur Android et intégration gameplay modèle par modèle.
