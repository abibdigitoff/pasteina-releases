# Nouveautés de PasteIna

Toutes les évolutions notables de PasteIna sont listées ici.

Le format suit [Keep a Changelog](https://keepachangelog.com/fr/1.1.0/) et les numéros de version suivent le [versionnage sémantique](https://semver.org/lang/fr/).

Les versions 0.1 à 0.4 sont des versions de développement internes : elles n'ont pas été publiées.

## [1.1.0] – 2026-10-28

### Modifié
- Nouveau design des cartes : icône de l'app à gauche, en-tête légèrement teinté, liseré de couleur, coins plus arrondis.
- Onglets des collections regroupés dans une barre unique, plus lisible.
- Réglages, écran de bienvenue et aperçu harmonisés avec ce nouveau style.
- Les téléchargements et les mises à jour sont désormais publiés sur le compte GitHub abibdigitoff.
- Nouveaux sons originaux de copie et de collage, activés par défaut.

### Corrigé
- Effets sonores : aucun son ne se jouait à la copie.

## [1.0.0] – 2026-10-28

Première version stable, validée après la bêta 0.9.0. Aucun changement fonctionnel depuis la 0.9.0.

## [0.9.0] – 2026-10-28

Bêta privée : étapes 0.5 (qualité et sécurité) et 0.9 (installation et mises à jour).

### Ajouté
- Coller plusieurs éléments à la suite : sélection multiple avec ⌘ ou ⇧.
- Réorganiser les collections par glisser-déposer.
- Effets sonores à la capture et au collage (réglage « Effets sonores »).
- Sauvegarde et restauration de l'historique et des collections (export / import).
- Mises à jour automatiques signées : PasteIna vérifie, télécharge et installe les nouvelles versions, en contrôlant leur signature.
- Journal d'erreurs local, consultable dans « À propos », pour aider à diagnostiquer un problème.
- Version universelle : une seule app pour les Mac Apple Silicon et Intel.

### Modifié
- La base de données utilise des migrations numérotées : une mise à jour ne fait jamais perdre l'historique.
- Les versions sont construites, signées, notarisées et publiées automatiquement depuis GitHub.

### Sécurité
- Interface verrouillée par une politique de sécurité du contenu (CSP) stricte : aucun script extérieur.
- Aucune connexion réseau en dehors de la vérification des mises à jour.
- Relecture de sécurité complète : presse-papiers, fichiers, base de données, commandes.

## [0.4.0] – 2026-10-27

### Ajouté
- Aperçu en grand avec la barre d'espace : texte complet, image en taille réelle.
- Modifier un élément texte avant de le coller (⌘E).
- Filtres de recherche par type (texte, image, lien, fichier, couleur) et par app d'origine.
- Glisser-déposer une carte vers n'importe quelle app.

### Modifié
- Police Poppins intégrée à l'app et appliquée à toute l'interface.

## [0.3.0] – 2026-10-27

### Ajouté
- Le panneau s'affiche au-dessus des apps en plein écran et sur tous les bureaux.
- Écran de bienvenue au premier lancement : présentation en trois étapes et demande guidée de l'autorisation Accessibilité, avec vérification en direct.
- Icône dans le Dock uniquement quand la fenêtre des réglages est ouverte.

### Modifié
- Grand historique fluide : seules les cartes visibles sont dessinées et l'historique se charge par pages (testé avec 10 000 éléments).
- Grosses images : une miniature est créée à la capture, l'original n'est chargé qu'au moment de coller.

## [0.2.0] – 2026-10-27

### Modifié
- Nouveau logo : deux anneaux imbriqués, bleu et orange.

### Ajouté
- Signature avec le certificat Developer ID d'ABIB DIGIT et Hardened Runtime.
- Script de publication : construction, signature, notarisation par Apple et agrafage du ticket au `.dmg`.

## [0.1.0] – 2026-10-27

Première version qui fonctionne de bout en bout.

### Ajouté
- Surveillance du presse-papiers : texte, texte mis en forme, images, fichiers, liens et couleurs.
- Historique enregistré localement (SQLite) et recherche instantanée qui ignore les accents.
- Collage direct dans l'app active.
- Panneau flottant animé avec des cartes, collections et menus natifs.
- Collage rapide (⌘1 à ⌘9) et collage en texte brut (⇧↩).
- Réglages : Général, Confidentialité, Raccourcis, À propos.
- Ouverture au démarrage du Mac et durée de conservation de l'historique.
- Pause de la capture, apps ignorées, contenus confidentiels et temporaires ignorés.
- Logo et icône dans la barre des menus.

[1.1.0]: https://github.com/abibdigitoff/pasteina-releases/releases/tag/v1.1.0
[1.0.0]: https://github.com/abibdigitoff/pasteina-releases/releases/tag/v1.0.0
[0.9.0]: https://github.com/abibdigitoff/pasteina-releases/releases/tag/v0.9.0
[0.4.0]: https://github.com/abibdigitoff/pasteina-releases/releases
[0.3.0]: https://github.com/abibdigitoff/pasteina-releases/releases
[0.2.0]: https://github.com/abibdigitoff/pasteina-releases/releases
[0.1.0]: https://github.com/abibdigitoff/pasteina-releases/releases
