---
id: catalog-volume-monitoring
themes: administration, akeneo-concepts, catalog-settings 
title: Controllr la **taille de votre catalogue** (since 2.3)
popular: false
related: what-is-a-product-value, what-is-an-attribute, what-is-a-family, what-is-a-channel, what-is-a-locale, what-is-a-category
---

# Un écran dédié

Un écran est disponible dans le PIM afin de controller la taille du catalogue sur plusieurs axes.

Cet écran contient par exemple le nombre de familles ou le nombre moyen d'attributs par famille.

![Catalog volume monitoring dashboard](../img/Activity_CatalogVolumeMonitoring_fr.png)

::: warning
Cet écran n'est disponible que depuis la version 2.3 du PIM.
:::

# Où est-ce?

Voici les étapes afin d'accéder à ce superbe (;)) écran:

1. Cliquer sur le menu `Activité`
2. Cliquer sur le sous-menu `Volume du catalogue`
3. Et voilà !

# Comment comprendre ce dashboard ?

## Les différentes sections

L'écran `Volume du catalogue` est composé de plusieurs sections.

### Le nombre de valeurs de produit

La première valeur affichée dans le widget représente le nombre total de [valeurs de produit](/articles/what-is-a-product-value.html) contenues dans le PIM.
C'est un indicateur de la valeur des données présentes dans votre catalogue produit. 

![Widget du nombre de valeurs de produit](../img/Activity_CatalogVolumeMonitoring_PvWidget_fr.png)

Nous vous encourageons à surveiller cette valeur régulièremeent. Plus le nombre de valeurs de produit est important, plus votre PIM vous est utile !

Nous avons écris un [article](https://medium.com/akeneo-labs/because-your-product-catalog-typology-matters-e1a9af4c33e0) en anglais afin d'expliquer pourquoi le nombre de valeurs produit est une métrique intéressante pour évaluer la taille de votre catalogue. Ne soyez pas effrayé par la taille de cet article ! Il mettra en lumière toute vos interrogations. Vous ne parlerez plus de la taille de votre catalogue de la même façon ;)

::: tips
Il se peut que le widget ne soit pas visible.
Si votre PIM est auto-hébergé ou bien en PAAS, c'est probablement parce que vous ou votre administrateur n'avez pas lancé le job quotidien de afin de calculer les valeurs du widget.

Afin de lancer ce job, veuillez vous référer à notre documentation technique [de la CE] (https://docs.akeneo.com/2.3/install_pim/manual/installation_ce_archive.html#configuring-tasks-via-crontab) ou bien [de la EE](https://docs.akeneo.com/2.3/install_pim/manual/installation_ee_archive.html#configuring-tasks-via-crontab).
:::

### Les autres sections

La prochaine section `Axes qui influencent le nombre de valeurs de produit` est dédié à plusieurs axes qui ont un impact sur le nombre de valeurs de produit total.
Par exemple, plus vous avez de canaux, plus le nombre de valeurs de produit sera élevé.

La section `Axes liés à la structure de votre catalogue` rassemble tous les axes ayant un impact sur la structure du catalogue, tel que le nombre de familles.

Enfin, la section `Axes concernant la modélisation des produits avec variantes` affiche le nombre de product models et le nombre de [produit variants](/articles/what-about-products-variants.html).

::: ee
Dans l'édition entreprise, une section additonnelle `Axes des assets` est présente. Celle-ci renseigne sur sur la volumétrie des [assets](/articles/work-with-assets.html) dans le PIM.
In the Entreprise Edition, there is an additional section called `Axes on assets` that will give you the volume regarding the [assets](/articles/work-with-assets.html).
:::

## Les alertes

Sur certains axes, vous observerez éventuellement des alertes. Celles-ci s'affichent derrière la métrique et l'icône de l'axe est alors affiché en violet. 
![Alerte dans l'écran de volumétrie du catalogue](../img/Activity_CatalogVolumeMonitoring_Alert_fr.png)

Cette alerte que la volumétrie correspondant à l'axe est élevée. Si vous rencontrez un problème concernant cet axe, veuillez nous contacter.
