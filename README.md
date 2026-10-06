# BE STRONGER — Espace Coach V13.6.9

Application web autonome pour gérer des fiches clients, suivre les séances, les performances et les règlements, et utiliser les timers d’entraînement.

## Lancer l’application

Ouvrir `index.html` dans un navigateur récent. Aucune installation n’est nécessaire.

## Données et sauvegardes

Les fiches clients, échéances et règlements sont conservés dans le stockage local du navigateur (`localStorage`). Ils restent sur l’appareil et le profil de navigateur utilisés. Depuis l’onglet **Clients**, exporter régulièrement une sauvegarde JSON. La restauration remplace les données présentes.

La V13.6.9 importe les fiches existantes au premier lancement dans son propre espace de stockage afin de garder la V13.6 originale intacte. Les données restent accessibles depuis l’application et ne sont pas synchronisées entre appareils. Ne pas publier de sauvegarde JSON ni de données client dans le dépôt GitHub.

## Suivi des règlements

Dans l’onglet **Paiements**, crée une échéance par client (prestation, montant, devise et date limite), enregistre les paiements totaux ou partiels, puis consulte le montant encaissé, le solde restant et les retards. Les règlements enregistrés peuvent être supprimés, ce qui recalcule le solde.

## Publier avec GitHub Pages

1. Créer un dépôt GitHub.
2. Ajouter `index.html` et `README.md` à la racine du dépôt.
3. Dans **Settings → Pages**, choisir **Deploy from a branch**, la branche `main` et le dossier `/ (root)`.
4. Enregistrer pour publier l’application.

## Timer

Le compte à rebours conserve le départ automatique après 10 secondes : bip à 3, 2 et 1, puis annonce « GO ». Le timer ajoute un bip sur chacune des 3 dernières secondes de chaque intervalle, phase ou échéance.


## Anneau du timer

L’anneau suit la progression du round courant : il se remplit à chaque intervalle EMOM et sur le round TABATA complet (effort + repos), puis repart au round suivant.


## Sens de progression de l’anneau

Le tracé du cercle progresse dans le sens inverse de la version précédente.


## Sens de progression de l’anneau

L’anneau démarre à 12 h et progresse dans le sens des aiguilles d’une montre jusqu’à compléter le round.


## Sens de progression de l’anneau

L’anneau démarre à 12 h et progresse dans le sens inverse des aiguilles d’une montre jusqu’à compléter le round.


## Annonces et bips

« HALF RIGHT THERE » est relancé proprement à la moitié de la durée. Les bips 3–2–1 marquent uniquement la fin du timer complet; les transitions de round gardent leur bip de repère.


« HALF RIGHT THERE » est annoncé à mi-round en EMOM et TABATA.
