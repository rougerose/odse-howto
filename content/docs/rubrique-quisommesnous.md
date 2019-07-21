---
title: Rubrique Qui sommes-nous ?
---
# Rubrique Qui sommes-nous ?

## Contenu de la rubrique
Cette rubrique présente le collectif et les associations membres. Elle fait l'objet d'un traitement particulier dans la mesure où elle affiche d'emblée l'intégralité du contenu de l'unique article auquel elle est liée.

{{< figure src="/docs/images/rubrique-quisommesnous.png" caption="Capture d'écran partielle de la rubrique Qui sommes-nous" class="capture" >}}

Les principes d'affichage des contenus de cette rubrique sont définis ainsi :

- Le champs ``Descriptif`` de la rubrique doit contenir un texte court de présentation de l'Observatoire. Ce texte court s'affiche sur [la page d'accueil du site](/docs/page-accueil/#présentation-de-l-odse) dans la zone relative à la présentation de l'ODSE.

- La rubrique ne doit contenir qu'**un seul article publié** et c'est son contenu qui sera affiché directement dans la page de la rubrique.

- Si le principe d'affichage du contenu de l'article est spécifique à cette rubrique, le contenu de l'article lui-même est commun à tous les articles du site. Il est donc possible d'utiliser toutes les ressources d'édition de texte et d'image disponible avec SPIP.

- Il n'existe qu'une seule exception au point précédent : il s'agit des associations membres qui apparaît sous le forme d'une liste horizontale (carrousel) que le visiteur peut faire défiler par la gauche ou par la droite. Cette liste présente pour chaque association : son logo (ou s'il n'est pas disponible un logo reprenant la lettre O du logo de l'ODSE), le nom de l'association et cet ensemble nom et logo est accompagné d'un lien vers le site de l'association membre (lorsqu'il existe).

- La liste des association est « alimentée » par la liste des sites référencés publiés dans la rubrique, comme le montre la capture ci-dessous.

{{< figure src="/docs/images/rubrique-quisommesnous-interface.png" caption="Capture d'écran de la rubrique Qui sommes-nous depuis l'interface privée du site. Dans le premier encadré rouge, l'unique article qui contient le texte de présentation de l'Observatoire. Dans le second encadré, la liste des sites référencés qui permet de constituer la liste des associations membres" class="capture" >}}

## La liste des associations membres
Pour constituer ou modifier la liste des associations membres, il est nécessaire de publier autant de « Sites référencés » que nécessaire. Les « Sites référencés » sont un type de contenu proposé par SPIP au même titre que les rubriques, les articles ou les mots-clés. Pour plus de détails sur la création ou l'édition des « Sites référencés », voir [la page de cette documentation qui y est consacrée](/docs/sites).


Pour faire apparaître la liste des associations membres à un emplacement précis du texte de présentation, il faut utiliser le principe d'« inclusion d'un modèle » (d'un code spécifique en d'autres termes) que propose SPIP (voir capture ci-dessous et en particulier l'encadré rouge).

{{< figure src="/docs/images/article-quisommesnous-edition.png" caption="Capture d'écran partielle du texte de présentation de l'Observatoire. En encadré rouge, le modèle qui permet de faire apparaître la liste des associations membres à un emplacement précis du texte." class="capture" >}}

Sur la capture ci-dessus, on constate que le modèle (ou code) consiste à écrire le texte suivant : ``<membres|titre=Les 29 associations membres de l'ODSE>``

La syntaxe est la suivante :

- le code doit être encadré des signes ``< >`` afin d'être interprété par SPIP comme tel, et non comme du texte courant.

- ``membres`` est le nom du modèle (ou du code) à inclure.

- le nom est suivi d'une barre verticale ``|`` (appelée aussi « tube » ou encore *pipe* en anglais) qui est disponible soit par la combinaison ``Alt Gr + 6`` (ordinateur sous Windows et Linux) ou la combinaison ``Alt + Maj + L`` (ordinateur sous OS X).

- La barre verticale est suivie du texte de l'intertitre qui apparaît juste au-dessus de la liste des logos des associations (voir la première capture en haut de cette page), ce texte doit être précédé de l'identifiant ``titre=``.

Ainsi, l'utilisation de ce « modèle » permet de faire apparaître la liste à l'emplacement souhaité et l'intertitre qui précède cette liste peut-être librement modifié.
