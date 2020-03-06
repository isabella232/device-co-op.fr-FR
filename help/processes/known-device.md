---
description: A propos des périphériques connus dans le graphique de périphériques.
seo-description: A propos des périphériques connus dans le graphique de périphériques.
seo-title: Périphériques connus
title: Périphériques connus
uuid: 53c21105-45b1-4bed-a473-d3ccc4bae965
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371

---


# Known devices{#known-devices}

A propos des périphériques connus dans le graphique de périphériques.

Device Graph repose sur le concept de *`known device`*. Un périphérique connu est un périphérique avec lequel un utilisateur interagit avec votre marque.

>[!NOTE]
>
>Dans le [!DNL Adobe Experience Cloud Device Co-op], termes tels que *`device`*, *`person`*, *`identity`* etc. ont des significations précises. Le terme « périphérique » peut, en effet, se rapporter au matériel (téléphone ou tablette) mais aussi aux applications qui s’exécutent sur ce matériel. Consultez le [glossaire](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c) pour en connaître les définitions.

## Supporting goals with the known device {#section-80deae33660e4280ac65c659ceff5601}

Le concept de périphérique connu s’accompagne de quelques objectifs essentiels à la création et à la maintenance d’un programme [!DNL Device Co-op] efficace. Un périphérique connu est un périphérique au sujet duquel un membre de [!DNL Device Co-op] possède des informations suite à une interaction avec un consommateur (visite d’un site ou utilisation d’une application mobile, par exemple). Based on these actions, the [!DNL Device Graph] links the known devices of a [!DNL Device Co-op] member to devices contributed by other [!DNL Device Co-op] members. Ces liens peuvent être [déterministes ou probabilistes](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931). This benefits [!DNL Device Co-op] members because they receive:

* davantage de données au sujet de leurs périphériques connus ;
* de nouvelles informations au sujet d’autres périphériques liés.

![](assets/known-device.png)

[!DNL Device Graph] ne divulgue jamais à un membre de Device Co-op donné des informations concernant des grappes de périphériques qu’il ne connaît pas.

## Device Co-op goals {#section-75aea5a102d54733aae2a7c6ee9ec6c7}

Three main goals animate the [!DNL Device Co-op]. à savoir : 

* **Échelle :** le partage du plus grand nombre de liaisons possibles à l’échelle de divers cas d’utilisation.
* **Équité :** chaque membre de [!DNL Device Co-op] profite des avantages de ce programme au prorata de sa contribution.

* **Confiance des consommateurs :** elle doit être établie et entretenue en s’assurant que l’expérience offerte aux consommateurs implique des marques qu’ils connaissent déjà et à qui ils font confiance, quel que soit le périphérique.

## Scale and the known device {#section-67f734109762457ca62ec306284ea082}

Les méthodes suivantes sont les méthodes les plus courantes pour qu’un périphérique soit qualifié de périphérique connu. Selon ces méthodes, les membres de [!DNL Device Co-op] disposent presque toujours d’au moins un périphérique connu conformément à l’objectif de fournir une échelle maximale à tous les membres de [!DNL Device Co-op].

**Organique**

* Suite à la visite d’un consommateur sur votre site ou à l’utilisation de votre application. Qualification découlant de données propriétaires.
* Enregistrement des consommateurs à partir d’un système de gestion des relations client (CRM).

**Marketplace**

* Achat des données de segments auprès d’Audience Marketplace.
* Suite à l’achat de données auprès d’un fournisseur de données tiers.

**Publicité**

Inventaire remporté lors d’une vente aux enchères et diffusion d’une publicité sur un périphérique. Le périphérique devient connu si cette publicité contient un pixel [!DNL Audience Manager].

## Known devices and fairness use cases {#section-0543188729d845d6b95db70b8b25e9f8}

Members of the [!DNL Device Co-op] get links commensurate with their contributions to the [!DNL Device Graph]. Les entreprises qui apportent à [!DNL Device Graph] des données sur de nombreux périphériques reçoivent davantage de liaisons que celles qui apportent des données sur quelques périphériques seulement. Ainsi, nous pensons que [!DNL Device Co-op] est équitable pour tous ses membres. Voyons comment ceci fonctionne avec les cas d’utilisation à grande et petite échelles décrits ci-après.

**Marque A : grand cas d&#39;utilisation**

Dans cet exemple, la marque A enregistre chaque mois 100 visiteurs sur son site et commence une nouvelle campagne multipériphérique. For simplicity, assume the [!DNL Device Graph] knows all of the visitors to Brand A are linked to 1 additional device. Cela signifie que la marque A pourrait atteindre 100 autres appareils. Additionally, the [!DNL Device Graph] contains about 200 devices linked together.

<table id="table_78C38DC522F94BC38C1DB73740C058AC"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Périphériques connus/mois </th> 
   <th colname="col2" class="entry"> Périphériques liés reçus de Device Co-op </th> 
   <th colname="col3" class="entry"> Total des périphériques pour la campagne </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>100 </p> </td> 
   <td colname="col2"> <p>100 </p> </td> 
   <td colname="col3"> <p>200 </p> </td> 
  </tr> 
 </tbody> 
</table>

**Marque B : cas d’utilisation à petite échelle**

Dans cet exemple, la marque B enregistre chaque mois 100 visiteurs sur son site et commence une nouvelle campagne multipériphérique. For simplicity, assume the [!DNL Device Graph] knows all of the visitors to Brand B are linked to 50 additional devices. La marque B peut donc atteindre 150 périphériques. Additionally, the [!DNL Device Graph] contains about 1,000 devices linked together.

<table id="table_A6C9CCF9C6564A89BA7060E075A8E73C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Périphériques connus/mois </th> 
   <th colname="col2" class="entry"> Périphériques liés reçus de Device Co-op </th> 
   <th colname="col3" class="entry"> Total des périphériques pour la campagne </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>100 </p> </td> 
   <td colname="col2"> <p>50 </p> </td> 
   <td colname="col3"> <p>150 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [Périphériques inconnus](../processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40)

