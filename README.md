# eimi-kill-switch

Ne sert qu'à une seule chose : signal d'auto-désactivation permanente de
l'application Android "Remontée Terrain EIMI" (dépôt privé séparé).

## Comment déclencher la désactivation

1. Sur ce dépôt GitHub, cliquer sur **Add file > Create new file**.
2. Nommer le fichier exactement `kill.html` (à la racine).
3. Mettre n'importe quel contenu (même vide) et valider ("Commit new file").
4. GitHub Pages republie en général sous 1 minute. L'application vérifie ce
   signal à chaque lancement : dès qu'elle détecte `kill.html`, elle se
   désactive **de façon permanente et irréversible** (même hors ligne, même
   si le fichier est supprimé ensuite) — seule une réinstallation complète
   de l'application la rétablit.

## Annuler avant déclenchement sur un appareil

Tant qu'un appareil n'a pas relancé l'application au moins une fois après la
création de `kill.html`, rien n'est encore déclenché dessus : supprimer le
fichier annule le signal pour les appareils qui ne l'ont pas encore vu.

URL vérifiée par l'application :
`https://willy059.github.io/eimi-kill-switch/kill.html`
