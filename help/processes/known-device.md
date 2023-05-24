---
description: À propos des appareils connus dans Device Graph.
seo-description: About known devices in the Device Graph.
seo-title: Known devices
title: Périphériques connus
uuid: 53c21105-45b1-4bed-a473-d3ccc4bae965
exl-id: 4eaf104f-022b-447b-8ce2-f0d0d1177cdf
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 1%

---

# Périphériques connus{#known-devices}

À propos des appareils connus dans Device Graph.

Dans Device Graph, nous avons le concept d’une *`known device`*. Un appareil connu est un appareil qu’un client utilise pour interagir avec votre marque.

>[!NOTE]
>
>Dans le [!DNL Adobe Experience Cloud Device Co-op], des termes tels que *`device`*, *`person`*, *`identity`* etc. ont des significations spécifiques. Par exemple, &quot;périphérique&quot; peut faire référence au matériel physique tel qu’un téléphone ou une tablette, ainsi qu’aux applications qui s’exécutent sur ce matériel. Voir [glossaire](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c) pour les définitions.

## Prise en charge des objectifs avec l’appareil connu {#section-80deae33660e4280ac65c659ceff5601}

Le concept d’appareil connu prend en charge quelques objectifs essentiels à la création et à la maintenance d’une [!DNL Device Co-op] programme. Un appareil connu est un appareil qu’un [!DNL Device Co-op] Le membre en sait plus sur une interaction avec un consommateur (par exemple, une visite de site ou l’utilisation d’une application mobile). En fonction de ces actions, la variable [!DNL Device Graph] relie les appareils connus d’une [!DNL Device Co-op] membre aux périphériques fournis par d’autres [!DNL Device Co-op] membres. Ces liens peuvent être [déterministe ou probabiliste](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931). Avantages [!DNL Device Co-op] membres car ils reçoivent :

* Plus de données sur leurs appareils connus.
* Nouvelles informations sur les autres appareils liés.

![](assets/known-device.png)

Le [!DNL Device Graph] ne fournira pas d’informations sur les grappes de périphériques qu’un membre de Device Co-op n’a pas vues.

## Objectifs de Device Co-op {#section-75aea5a102d54733aae2a7c6ee9ec6c7}

Les trois principaux objectifs de la [!DNL Device Co-op]. Ces cas comprennent notamment :

* **Échelle :** Partagez le nombre maximum de liens possibles dans divers cas d’utilisation.
* **Équité :** Assurez-vous que chaque membre du [!DNL Device Co-op] d&#39;une manière proportionnelle à leurs contributions.

* **Confiance des consommateurs :** Maintenir et renforcer la confiance des consommateurs en s’assurant que l’expérience des consommateurs sur plusieurs appareils implique des marques qu’ils connaissent déjà et qu’ils ont confiance.

## Échelle et périphérique connu {#section-67f734109762457ca62ec306284ea082}

Les méthodes suivantes sont les méthodes les plus courantes qu’un appareil peut qualifier d’appareil connu. Compte tenu de ces méthodes, [!DNL Device Co-op] Les membres auront presque toujours au moins un appareil connu. Cela prend en charge l’objectif de fournir une échelle maximale à tous les membres de la variable [!DNL Device Co-op].

**Organique**

* De la visite d’un client sur votre site ou en utilisant votre application. Il s’agit d’une qualification à partir de données propriétaires.
* par les clients intégrés à partir d’un système CRM ;

**Marketplace**

* Achat de données de segment à partir d’une Audience Marketplace.
* d’acheter des données auprès d’un fournisseur de données tiers ;

**Publicité**

En gagnant l’inventaire lors d’une vente aux enchères et en diffusant une publicité sur un appareil. L’appareil devient un appareil connu si cette publicité contient une [!DNL Audience Manager] pixel.

## Périphériques connus et cas d’utilisation de l’équité {#section-0543188729d845d6b95db70b8b25e9f8}

Les membres de [!DNL Device Co-op] obtenir des liens proportionnés à leurs contributions à la variable [!DNL Device Graph]. Sociétés qui apportent de nombreux appareils au [!DNL Device Graph] recevoir plus de liens que les membres qui ne contribuent que quelques uns. Nous pensons que cela aide à [!DNL Device Co-op] juste pour tous ses membres. Examinons comment cela fonctionne avec les cas d’utilisation petits et grands décrits ci-dessous.

**Marque A : cas pratique important**

Dans cet exemple, la marque A reçoit 100 visiteurs par mois et lance une nouvelle campagne sur plusieurs appareils. Pour plus de simplicité, supposons que la variable [!DNL Device Graph] sait que tous les visiteurs de la marque A sont liés à 1 périphérique supplémentaire. Cela signifie que la marque A peut atteindre 100 autres périphériques. En outre, la variable [!DNL Device Graph] contient environ 200 appareils liés ensemble.

<table id="table_78C38DC522F94BC38C1DB73740C058AC"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Périphériques/mois connus </th> 
   <th colname="col2" class="entry"> Périphériques liés reçus de Device Co-op </th> 
   <th colname="col3" class="entry"> Nombre total de périphériques pour Campaign </th> 
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

**Marque B : Petit cas d’utilisation**

Dans cet exemple, la marque B reçoit 100 visiteurs par mois et lance une nouvelle campagne sur plusieurs appareils. Pour plus de simplicité, supposons que la variable [!DNL Device Graph] sait que tous les visiteurs de la marque B sont liés à 50 appareils supplémentaires. Cela signifie que la marque B peut atteindre 150 périphériques. En outre, la variable [!DNL Device Graph] contient environ 1 000 appareils liés ensemble.

<table id="table_A6C9CCF9C6564A89BA7060E075A8E73C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Périphériques/mois connus </th> 
   <th colname="col2" class="entry"> Périphériques liés reçus de Device Co-op </th> 
   <th colname="col3" class="entry"> Nombre total de périphériques pour Campaign </th> 
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

