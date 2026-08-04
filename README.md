# Horsevo — tableau de bord de lancement

Page statique qui affiche en direct les inscriptions à [Horsevo](https://apps.apple.com/app/id6760648026).

## Sécurité

Ce dépôt ne contient **aucun secret**. La page lit son jeton d'accès dans le
fragment de l'URL (la partie après `#`), qui n'est ni envoyé au serveur ni
stocké ici. Ouverte sans ce fragment, elle n'affiche rien.

Les données proviennent d'une fonction Postgres `live_stats` qui ne renvoie que
des agrégats et des prénoms : aucune adresse e-mail, aucun numéro de téléphone.
