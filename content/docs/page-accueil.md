---
title: Page d'accueil
---
# Page d'accueil du site
La page d'accueil du site est divisée en 3 zones (voir capture d'écran ci-dessous) :

1. Articles sélectionnés
2. Présentation de l'ODSE
3. Derniers articles d'actualités

{{< figure src="/docs/images/page-accueil.png" class="capture" >}}

## Articles sélectionnés
Cette zone repose sur un principe d'affichage d'articles triés selon une sélection établie par les responsables du site (sélection manuelle), ou, si cette sélection est vide, une sélection automatique d'articles établie selon des critères prédéfinis.

### Sélections manuelles
Lorsque la [sélection éditoriale](/docs/selections) dédiée à la page d'accueil contient au moins un article, elle s'affiche de manière prioritaire.

Ce principe de sélection manuelle permettra d'afficher les articles que l'on souhaite accompagné (ou pas) d'une image, d'un résumé spécifique à la page d'accueil et dans l'ordre que l'on souhaite.

Cette sélection peut être modifiée autant de fois que nécessaire.

Les principes d'affichage sont détaillés dans la page de documentation des [sélections éditoriales](/docs/selections).

### Sélections automatiques
Si l'on préfère afficher les derniers articles publiés sur le site, dans l'ordre chronologique décroissant de leur date de publication, il suffit de s'assurer que la sélection dédiée à la page d'accueil soit vide de tout article et l'affichage automatique aura alors la priorité.

Les critères d'affichage sont les suivants :

- Seuls les articles publiés dans les rubriques **S'informer** et **Nos actions** sont pris en compte.
- Puis ils sont triés par ordre chronologique décroissant de leur date de publication (le plus récent en premier, le plus ancien en dernier).
- Le titre est identique à celui de l'article.
- Le résumé peut avoir deux sources différentes : si le champ ``Descriptif`` de l'article est rempli, c'est lui qui est utilisé en priorité. Si le ``Descriptif`` est vide, SPIP affiche les 300 premiers caractères de l'article.
- Si l'article est accompagné d'un ``Logo d'article``, il est affiché.


## Présentation de l'ODSE
Cette zone permet d'afficher un court résumé de présentation du collectif.

Ce resumé correspond au champ ``Descriptif`` de [la rubrique **Qui sommes-nous ?**](/docs/rubrique-quisommesnous).


## Actualités
Cette zone affiche selon un principe automatique les **5** derniers articles publiés dans la rubrique **Actualités**.

Au-dessus de la liste de ces articles, une phrase d'introduction du contenu (« L'actualité des associations membres de l'ODSE ») est également affichée. Cette phrase est enregistrée dans le champ ``Descriptif`` de la rubrique **Actualités**.

Les principes d'affichage des contenus (date, nom de l'organisation source de l'article, titre) sont détaillés dans la page de documentation de la rubrique [**Actualités**](/docs/rubrique-actualites).
