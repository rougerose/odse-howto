---
title: Pied de page
---
# Pied de page
En bas de chaque page, un bloc identique est inséré et contient :

- le nom développé de l'ODSE.
- de liens directes vers les pages ``Contacter l'ODSE`` et ``Mentions légales``.

{{< figure src="/docs/images/pied.png" class="capture" caption="Pied de page. Le lien Mentions légales n'est pas apparent car la page n'est pas publiée au moment de la rédaction de cette documentation." >}}

## Nom développé de l'ODSE
Le nom développé de l'ODSE (Observatoire du droit à la santé des étrangers) correspond au ``Nom du site``, champ de saisie disponible dans la page ``Configuration > Identité du site``.

## Pages Contacter l'ODSE et Mentions légales
Ces pages correspondent des ``Articles uniques``, articles d'un format particulier puisqu'ils ne dépendent d'aucune rubrique du site.

Ces articles sont accessibles depuis l'entrée ``Édition > Pages uniques`` de l'interface privée.

Chacun de ces articles est associé à un *identifiant spécifique* (champ ``Page`` de chaque article) qui permet à SPIP de différencier ces deux pages. Il est donc indispensable que la page **Contacter l'ODSE** possède l'identifiant ``contact`` et la page **Mentions légales** l'identifiant ``mentions``.
