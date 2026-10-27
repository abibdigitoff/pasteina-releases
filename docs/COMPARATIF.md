# Comparatif : PasteIna et Paste

[Paste](https://pasteapp.io) est le gestionnaire de presse-papiers de référence sur Mac. PasteIna s'en inspire. Cette page compare les deux apps, chiffres à l'appui, le plus honnêtement possible.

**En bref :** Paste est plus complet (synchronisation iCloud, app iPhone et iPad, plus de fonctions) et payant par abonnement. PasteIna est gratuit, environ 5 fois plus petit, utilise environ 4 fois moins de mémoire et garde tout sur votre Mac.

## Chiffres

| Mesure | Paste | PasteIna |
| --- | --- | --- |
| Taille de l'app installée (`.app`) | 33 Mo | **6,6 Mo** |
| Taille du téléchargement (`.dmg`) | non mesuré | **3,2 Mo** |
| Mémoire utilisée (processus principal) | ~330 Mo | **~75 Mo** |

### Performances de PasteIna avec un gros historique

Test réalisé avec **10 000 éléments** dans l'historique :

| Opération | Résultat |
| --- | --- |
| Enregistrer un nouvel élément | ~385 µs par élément |
| Rechercher | 0,2 à 5 ms |
| Afficher une page loin dans l'historique (à partir du 9 800ᵉ élément) | 2 ms |
| Taille de la base de données | 9,9 Mo |

Une recherche en moins de 5 ms est imperceptible : les résultats s'affichent pendant la frappe. Paste n'a pas été soumis au même test (sa base de données n'est pas accessible de la même façon), ces chiffres ne servent donc pas de comparaison directe.

## Fonctions

| Fonction | Paste | PasteIna |
| --- | --- | --- |
| Texte, texte mis en forme, images, fichiers, liens, couleurs | Oui | Oui |
| Recherche instantanée | Oui | Oui (accents ignorés) |
| Filtres par type et par app | Oui | Oui |
| Collections (pinboards) | Oui | Oui |
| Aperçu en grand (barre d'espace) | Oui | Oui |
| Modifier avant de coller | Oui | Oui |
| Glisser-déposer | Oui | Oui |
| Collage rapide (⌘1…9) et texte brut | Oui | Oui |
| Apps ignorées, contenus confidentiels ignorés | Oui | Oui |
| Coller plusieurs éléments à la suite | Oui | Prévu pour la 1.0 |
| Sauvegarde et restauration | – | Prévu pour la 1.0 |
| Pile de collage (copier plusieurs, coller dans l'ordre) | Oui | Idée pour après la 1.0 |
| Aperçu des liens (image et titre de la page) | Oui | Idée pour après la 1.0 |
| Synchronisation iCloud entre appareils | **Oui** | Non |
| App iPhone et iPad | **Oui** | Non |
| Interface en plusieurs langues | Oui | Français uniquement |
| Prix | Abonnement payant | **Gratuit** |
| Où sont les données | Sur le Mac, et dans iCloud si la synchronisation est activée | **Uniquement sur le Mac** |
| Compte nécessaire | Pour la synchronisation | **Jamais** |

« – » signifie « non vérifié ». La liste des fonctions de Paste est donnée à titre indicatif et peut évoluer : consultez [pasteapp.io](https://pasteapp.io) pour l'offre et le tarif actuels.

## Lequel choisir ?

- **Choisissez Paste** si vous voulez retrouver votre historique sur plusieurs Mac, sur iPhone ou sur iPad, ou si vous utilisez ses fonctions avancées.
- **Choisissez PasteIna** si vous utilisez un seul Mac, voulez une app gratuite et légère, et préférez que rien ne quitte votre ordinateur.

## Méthode de mesure

- **Date :** 27 octobre 2026.
- **Machine :** Mac Apple Silicon, macOS 26.
- **Versions :** PasteIna 0.4 (version de développement, compilée en mode publication, architecture arm64) ; Paste dans sa version disponible à cette date.
- **Taille de l'app :** `du -sh` sur le dossier `.app` installé dans `/Applications`. La taille de PasteIna correspond à la version Apple Silicon seule ; la future version universelle (Apple Silicon + Intel) sera un peu plus grosse.
- **Mémoire :** mémoire résidente (RSS) relevée avec `ps -o rss,comm` sur le **processus principal** de chaque app, ouverte et au repos, après utilisation normale. Le processus WebKit qui dessine l'interface de PasteIna n'est pas compté, pas plus que les processus annexes de Paste. La mémoire varie selon la taille de l'historique et l'usage : ces valeurs sont des ordres de grandeur, pas des chiffres exacts.
- **Performances :** test automatique sur la base de données de PasteIna, remplie avec 10 000 éléments générés, sur la même machine.

PasteIna n'est pas affilié à Paste ni à ses éditeurs. « Paste » est une marque de ses propriétaires respectifs.
