---
title: Les articles
---
# Les articles et leur mise en forme

Cette page décrit les différentes possibilités de mise en forme des articles sur le site, soit avec l'aide des fonctions standards de SPIP (et qui sont également détaillées [dans la documentation de l'outil](/docs/spip_documentation)).

Toutes les informations développées ici se basent sur un article fictif publié dans une version de développement du site (voir ci-dessous la capture partielle de cet article). Compte tenu du fait que cette documentation repose sur un outil différent de SPIP et que les règles de mise en page ne sont pas celles utilisées sur le site de l'ODSE, chaque code ou raccourcis présenté ici sera accompagné d'une capture afin de mettre en évidence d'un côté le code et de l'autre sa traduction graphique.

{{< figure src="/docs/images/article-partiel.png" class="capture" caption="Capture partielle d'un article fictif qui présente un large éventail des possibilités de mise en forme d'un article." >}}

# Entête

{{< figure src="/docs/images/article-entete.png" class="capture" caption="Entête de l'article." >}}

## Date de publication
La date de publication en ligne de l'article est affichée en haut à gauche.

## Information validité de l'article
Lorsque la date de l'article comparée à la date de consultation de l'article est supérieure à un délai défini par les responsables du site, un bandeau d'information s'affiche automatiquement. Pour plus d'information à ce sujet, voir [cette page](/docs/article-validite).

# Titre et logo de l'article

{{< figure src="/docs/images/article-titre.png" class="capture" caption="Entête de l'article." >}}

## Titre, surtitre et sous-titre
En plus du titre, il est d'utiliser un surtitre et un sous-titre.

## Logo d'article
L'article peut être « introduit » par une image grand format, qui, selon la terminologie utilisée par SPIP, est utilisée comme ``Logo d'article``.

Cette image devra être traitée et reformatée avant d'être importée sur le site. La largeur optimum de cette image sera de 700 pixels. Voir [cette page pour des informations supplémentaires sur le traitement des images](/docs/images).

# Corps de l'article

## Chapeau
Le texte proprement dit de l'article peut être précédé d'un ou plusieurs paragraphes de présentation ou d'introduction. Cette introduction est appelé ``chapeau``. Un champ spécifique dans le formulaire d'édition de l'article permet d'utiliser cette possibilité.

Le chapeau sera présenté selon une taille de caractère sensiblement plus importante que le corps du texte.

{{< figure src="/docs/images/article-chapo.png" class="capture" caption="Le chapeau de l'article suivi d'un corps de l'article -- qui débute par un intertitre. Le chapeau est affiché dans une taille de caractère plus grande que les paragraphes du corps du texte." >}}

## Structurer un texte

Il est important de prendre soin à la structure du texte que l'on adopte. Cette structure correctement établie permettra de donner au texte une forme qui facilite la lecture, mais elle aura aussi des conséquences sur un balisage approprié du texte.

Trois exemples assez fréquents pour illustrer cette question :

Premier exemple, deux paragraphes sont saisis à la suite et un seul retour de chariot les sépare. Le code HTML produit par cette saisie correspond un unique paragraphe au lieu de deux. Il faudra donc séparer chaque paragraphe d'un double retour de chariot afin que le code HTML soit correct et que chaque paragraphe soit balisé individuellement.

Deuxième exemple, une erreur assez courante est de mettre un intertitre en gras. Si, visuellement, cela peut être suffisant, le balisage (HTML) est erroné : la phrase ou les quelques mots en gras qui devraient être balisés comme un intertitre sont en fait balisés comme un paragraphe mis en gras.

Troisième exemple : les différents paragraphes d'une liste sont parfois précédés d'un simple tiret. Visuellement cela peut suffire mais structurellement le balisage est incorrect car il s'agit d'un simple paragraphe qui débute par un tiret, alors qu'il devrait être balisé avec les balises spécifiques d'une liste.

Sans rentrer davantage dans les détails techniques, il est important que les personnes chargées de la rédaction ou de la mise en ligne des articles utilisent toutes les possibilités de raccourcis qu'offre SPIP (et le HTML d'une manière générale) pour préparer le texte, ce qui facilitera la mise en forme, mais aussi la lecture et l'indexation des articles par les moteurs de recherche.

## Paragraphes

La gestion des paragraphes, et en particulier l'importance des espaces blancs entre deux paragraphes, est expliquée [dans la documentation standard de SPIP](/docs/spip_documentation).

## Intertitres
Lorsque le texte fait apparaître des intertitres, il faut utiliser les raccourcis qui permettent de baliser les intertitres.

Le HTML possède 5 niveaux d'intertitres, et SPIP propose autant de raccourcis pour les utiliser :

1. Le premier niveau d'intertitre sera saisi ainsi : ``{{{ texte de l'intertitre de premier niveau }}}`` ou ``{{{* texte de l'intertitre de premier niveau }}}``. Soit trois accolades suivies d'une astérisque.

2. Le second niveau : ``{{{** texte de l'intertitre de second niveau }}}``. Soit trois accolades suivies de deux astérisques.

3. Le troisième niveau : ``{{{*** texte de l'intertitre de premier niveau }}}``. Soit trois accolades suivies de trois astérisques.

4. Le quatrième niveau : ``{{{**** texte de l'intertitre de quatrième niveau }}}``. Soit trois accolades suivies de quatre astérisques.

5. Le cinquième et dernier niveau : ``{{{***** texte de l'intertitre de premier niveau }}}``. Soit trois accolades suivies de cinq astérisques.


Ce qui se traduit visuellement par ceci :

{{< figure src="/docs/images/article-intertitres.png" class="capture" caption="Les différents niveaux d'intertitres d'un texte." >}}

## Gras et italique

SPIP propose des « raccourcis » (ou codes qui lui sont spécifiques) afin de pouvoir mettre certains passage d'un texte en gras ou en italique.

Pour **l'italique** : le passage qui apparaîtra en italique sera entouré d'une accolade ``{texte en italique}``.

Pour **le gras** : le passage qui apparaitra en gras sera entouré de deux accolades ``{{texte en gras}}``.

Pour un passage en gras **et** en italique : il suffit de cumuler les deux raccourcis en prenant garde de les séparer d'une espace ``{{ {texte en gras et en italique} }}``.

## Liens

Il existe un raccourci spécifique qui permet de réaliser des liens.

Si l'on souhaite placer un lien sur un mot ou un groupe de mots, le raccourci est le suivant : ``Consulter [cette page->adresse de la page] pour plus d'informations``.

Ensuite, il convient de différencier deux types de liens possibles : s'agit-il de proposer un **lien interne** ou **un lien externe** ?

### Liens internes
Dans le premier cas, vous souhaitez faire un lien vers un autre article du site de l'ODSE, ou une rubrique du site, ou un mot-clé ou un document… En d'autres termes, vous souhaitez faire un lien vers **un contenu du site** qui a été publié à l'aide de SPIP.

Dans ce cas, il **ne faut pas récupérer l'adresse publique** du contenu (adresse qui commence par https://odse.eu.org/...), il est préférable d'utiliser la **référence interne** au contenu : tous les éléments (contenus) publiés avec SPIP sont identifié par un nom (rubrique, article, document, mot, etc.) et un numéro d'identification qui lui est propre. Ce numéro est toujours affiché sur la page de prévisualisation de l'élément en haut à gauche.

Pour reprendre l'exemple ci-dessus et si l'on souhaite faire un lien vers un autre article, il faudra alors écrire : ``Consulter [cette page->articleXX] pour plus d'informations.`` et remplacer ``XX`` par le numéro d'identification de l'article. Ou si l'on souhaite faire un lien vers un document PDF qui a été mis en ligne dans le même article (ou tout autre article du site), il suffit de noter son numéro d'identification et d'écrire ``Consulter [ce document PDF->documentXX] pour plus d'informations``.

À noter qu'il existe une variante possible qui permet à la fois de créer un lien et de récupérer le titre du contenu (à condition que le champ titre existe et qu'il soit rempli). Ainsi, si l'on souhaite faire un lien vers l'article 139 du site dont le titre est « Inclure l’Aide médicale de l’État (AME) dans le régime général de Sécurité sociale » et que l'on écrit ``Consulter notre article « [->article139] »``, SPIP affichera ensuite ceci : Consulter notre article [« Inclure l’Aide médicale de l’État (AME) dans le régime général de Sécurité sociale »](https://www.odse.eu.org/spip.php?article139).

### Liens externes
S'il s'agit de réaliser un lien externe vers le site « Nom-de-domaine.com », le raccourci est le suivant : ``Consulter [ce site->http://nom-de-domaine.com] pour plus d'informations``.

## Listes
Deux raccourcis existent pour écrire des listes : liste non ordonnée ou ordonnée avec numéro.

### Liste non ordonnée

Le raccourci pour écrire une liste non ordonnée est `-*`. Il est possible de créer des listes imbriquées de la manière suivante :
```
-* Élément de liste non numérotée
-* Élément de liste non numérotée
-* Élément de liste non numérotée
-** Plantes
-*** Ficus
-*** Olivier
-** Animaux de compagnie
-*** Chat
-*** Chien
```

### Liste ordonnée

Le raccourci pour écrire une liste ordonnée est `-#`. Il est possible d'imbriquer des listes numérotées de la même manière que les listes non ordonnées (`-##` pour un élément de niveau deux par exemple).

{{< figure src="/docs/images/article-listes.png" class="capture" caption="Les listes ordonnées et non ordonnées." >}}

## Tableaux

Il est possible de créer des tableaux (simples). Pour les tableaux complexes ou qui contiennent un grand nombre de données, il est préférable d'envisager d'autres principes de mise en ligne (pages développées de manière spécifique ou plus simplement annexer un tableau complexe dans un document PDF par exemple).

Pour créer un tableau, les raccourcis sont les suivants :
```
||Titre du tableau ||
|{{entête}}|{{entête}}|{{entête}}|
| valeur | valeur | valeur |
| valeur | valeur | valeur |
| valeur | valeur | valeur |
```

À noter que les barres verticales qui forment chaque cellule du tableau sont saisies soit par la combinaison ``Alt Gr + 6`` (ordinateur sous Windows et Linux), soit la combinaison ``Alt + Maj + L`` (ordinateur sous OS X).

Ce qui est affiché ainsi par SPIP :

{{< figure src="/docs/images/article-tableaux.png" class="capture" caption="Les tableaux." >}}


## Citations

Les citations peuvent être saisies de la manière suivante :

- Pour une citation incluse dans un paragraphe, on écrira : `Et il s'écria : <q>« La route est longue mais la voie est libre »</q>`.

- Pour une citation isolée et qui comprend un ou plusieurs paragraphes, on écrira :
```
<quote>Premier paragraphe : La route est longue mais la voie est libre.

Second paragraphe : Deux humains s'échangent une pièce de 1€ […]</quote>
```

À noter qu'il est aussi possible d'utiliser directement le code HTML `<blockquote> </blockquote>` à la place de `<quote> </quote>`.

{{< figure src="/docs/images/article-citations.png" class="capture" caption="Les citations." >}}

## Les notes de bas de page

Les notes sont saisies par l'intermédiaire d'un raccourci que l'on place à l'endroit où l'appel de note doit apparaître :

`Proin porttitor, orci nec nonummy molestie, enim est eleifend mi, non fermentum diam nisl sit amet erat[[Texte de la note]]. Duis semper. Duis arcu massa, scelerisque vitae, consequat in, pretium a, enim. Pellentesque congue.`

Qui sera traduit dans le second paragraphe de la capture ci-dessous :

{{< figure src="/docs/images/article-notes.png" class="capture" caption="Les notes. Le texte de la note est affichée en bas de l'article et n'est pas visible sur cette capture." >}}

## Mise en forme à l'aide de balises HTML

Certaines balises HTML n'existent pas sous forme de raccourcis SPIP, mais certaines d'entre elles peuvent être utiles comme les exposants ou les indices :

- exposant : `Le XX<sup>e</sup> siècle` Le XX<sup>e</sup> siècle.
- indice : `La formule brute de l'eau s'écrit H<sub>2</sub>O` La formule brute de l'eau s'écrit H<sub>2</sub>O

## Les images et documents

En dehors des logos d'article (voir plus haut dans cette page), des images et des documents (PDF par exemple) peuvent être insérés dans le texte ou associés comme documents joints. Dans ce dernier cas, ils apparaitront après le corps de l'article.

### Importer une image ou un document
Avant d'importer une image ou un document, il est important de préparer le fichier afin qu'il soit le plus léger possible et adapté à une consultation en ligne. Par exemple, il est préférable de mettre à disposition un fichier PDF plutôt qu'un fichier .doc, ce dernier nécessitant une application de traitement de texte pour être lu alors que le PDF sera affiché directement par le navigateur.

Pour les informations plus détaillées concernant le traitement préalable et la taille des images, voir [la page de cette documentation](/docs/images) consacrée à cet aspect.

Pour importer un document (ou une image), il est possible de le faire depuis la page des **Documents** de SPIP (accessible par l'entrée `Édition > Documents`) ou au moyen du formulaire de téléchargement notamment disponible en bas de la page de prévisualisation d'un article.

À noter que lorsqu'un document a été téléchargé sur le site par l'intermédiaire du site et que l'on souhaite l'utiliser dans plusieurs articles, il n'est pas nécessaire de le télécharger plusieurs fois. Il suffit de le sélectionner à nouveau par l'intermédiaire du formulaire de téléchargement d'un article et de choisir l'option `Depuis la médiathèque` et, si l'on ne connait pas le numéro d'identification du document, de cliquer sur le bouton `Parcourir`.

### Images insérées

Pour insérer une image dans le corps de l'article, il suffit de saisir le raccourci suivant `<docXX>` (remplacer XX par le numéro d'identification du document).

Pour aligner l'image au centre de la page, à gauche ou à droite (par rapport au texte de l'article), le raccourci sera à compléter de par l'indication d'alignement souhaité (en anglais) : `<docXX|center>` (pour une image au centre), `<docXX|left>` (image calée à gauche) ou `<docXX|right>` (image calée à droite).

Comme le montre la capture ci-dessous, l'image est dans tous les cas affichée par SPIP dans un format réduit automatiquement.

{{< figure src="/docs/images/article-images.png" class="capture" caption="Les images insérées dans le corps de l'article." >}}

Mais il reste possible d'afficher les images dans une taille plus grande (mais qui n'excédera pas la largeur de la colonne de texte de l'article, soit 700 pixels au maximum). Pour cela, il faudra utiliser le raccourci `<docXX|img>` ou `<docXX|emb>`. Le premier affiche l'image sans légende (qu'elle existe ou pas) alors que le second l'affichera.

{{< figure src="/docs/images/article-images2.png" class="capture" caption="Les images insérées dans le corps de l'article." >}}

### Images et documents associés à un article

Lorsque les documents ne sont pas utilisés comme **illustrations** selon la terminologie de SPIP (c'est-à-dire insérés dans le corps de l'article), ils sont alors considérés comme des **documents associés** à un article et ils apparaissent en bas de l'article, comme le montre la capture ci-dessous.

{{< figure src="/docs/images/article-documents.png" class="capture" caption="Les documents (images et PDF) associés à un article." >}}
