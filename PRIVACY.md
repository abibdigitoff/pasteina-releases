# Politique de confidentialité de PasteIna

*Dernière mise à jour : 27 octobre 2026*

PasteIna est édité par ABIB DIGIT. En une phrase : **tout ce que PasteIna enregistre reste sur votre Mac, et rien ne nous est envoyé.**

## Ce que PasteIna enregistre

Pour fonctionner, PasteIna garde une copie de ce que vous copiez : textes, images, fichiers, liens et couleurs, avec le nom de l'app d'où ils viennent et l'heure de la copie. Il enregistre aussi vos collections et vos réglages.

Tout est rangé **uniquement sur votre Mac**, dans ce dossier :

```
~/Library/Application Support/com.pasteina.desktop/
```

Rien n'est copié ailleurs : ni sur un serveur, ni dans iCloud, ni chez ABIB DIGIT.

## Ce que PasteIna n'enregistre pas

PasteIna ignore automatiquement :

- **les contenus confidentiels** : les mots de passe et données que les autres apps marquent comme secrets (norme `org.nspasteboard.ConcealedType`, utilisée par la plupart des gestionnaires de mots de passe, dont 1Password) ;
- **les contenus temporaires** : les données que les apps marquent comme transitoires ou générées automatiquement ;
- **les apps ignorées** : par défaut, l'app **Mots de passe** et **Trousseaux d'accès** d'Apple. Vous pouvez en ajouter d'autres dans **Réglages → Confidentialité → Ignorer les applications** ;
- **tout ce qui est copié pendant une pause** de la capture.

Ces protections sont activées par défaut et réglables dans **Réglages → Confidentialité**.

## Pas de compte, pas de statistiques

- Aucun compte n'est nécessaire.
- Aucune statistique d'utilisation, aucune mesure d'audience, aucun pistage, aucune publicité.
- Aucun rapport de plantage n'est envoyé. Si un journal d'erreurs existe, il reste sur votre Mac ; c'est vous qui décidez de nous le transmettre.

## La seule connexion réseau : les mises à jour

PasteIna se connecte à Internet pour une seule raison : **vérifier s'il existe une nouvelle version**, et la télécharger si c'est le cas. Il interroge pour cela les serveurs de **GitHub**, où sont publiées les versions de PasteIna.

Ce qui est envoyé : une requête web standard, qui ne contient **aucune donnée de votre historique**, aucun identifiant personnel et aucune information sur votre utilisation. Comme pour toute visite d'un site web, GitHub voit votre adresse IP et des informations techniques de base (version de l'app, système). Ces données sont traitées par GitHub selon sa propre [déclaration de confidentialité](https://docs.github.com/fr/site-policy/privacy-policies/github-general-privacy-statement). ABIB DIGIT n'y a pas accès.

## Autorisation Accessibilité

PasteIna demande l'autorisation **Accessibilité** de macOS pour une seule chose : simuler ⌘V afin de coller l'élément choisi dans l'app que vous utilisez. Il ne lit pas ce que vous tapez et n'enregistre pas vos frappes. Vous pouvez retirer cette autorisation à tout moment dans **Réglages Système → Confidentialité et sécurité → Accessibilité**.

## Supprimer vos données

- **Effacer l'historique :** **Réglages → Général → Effacer l'historique…** (les éléments rangés dans des collections sont conservés).
- **Supprimer un élément :** sélectionnez-le dans le panneau et appuyez sur ⌘⌫.
- **Limiter la conservation :** **Réglages → Général → Conserver l'historique** (un jour, une semaine, un mois, un an ou toujours). Les éléments plus anciens sont effacés automatiquement, sauf ceux rangés dans une collection.
- **Tout supprimer :** quittez PasteIna et supprimez le dossier `~/Library/Application Support/com.pasteina.desktop/`. La procédure de désinstallation complète est dans la [FAQ du README](README.md#questions-fréquentes).

Comme vos données ne sont stockées que sur votre Mac, ABIB DIGIT ne peut ni les consulter, ni les supprimer, ni les récupérer pour vous. Pensez à la sauvegarde de votre Mac (Time Machine, par exemple) si votre historique vous est précieux.

## Contact

Une question sur cette politique ? Ouvrez un ticket sur [GitHub](https://github.com/adidiibou0218-ui/pasteina-releases/issues).

Si cette politique change, la nouvelle version sera publiée ici, avec sa date.
