---
description: Descriptions et réponses aux questions courantes sur la coopération Identity Services et le graphique d'identité.
seo-description: Descriptions et réponses aux questions courantes sur la coopération Identity Services et le graphique d'identité.
seo-title: FAQ
title: FAQ
uuid: 490566e1-4d35-468c-8389-678f9ff02cc8
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---


# FAQ{#faq}

Descriptions et réponses aux questions courantes sur la coopération Identity Services et le graphique d&#39;identité.

**Quel est le  [!DNL Device Co-op]?**

Device Co-op est une coopérative numérique qui permet aux clients Adobe Experience Cloud participants de travailler ensemble pour mieux identifier leurs consommateurs sur les différents appareils.

**Quelles technologies sont utilisées dans Device Co-op ?**

Device Co-op est constitué de deux technologies :

* **Service d’identification des Experience Cloud :** ce service principal du Adobe Experience Cloud fournit un ID commun permettant d’identifier les consommateurs de manière cohérente entre les solutions, les canaux, les expériences et les périphériques.
* **Adobe Experience Cloud Device Co-op :** cette technologie relie différents appareils utilisés par un consommateur ou un ménage.

**Comment ça  [!DNL Device Co-op] marche ?**

Alors que les marques lancent dans leur pièce du puzzle sur plusieurs périphériques par le biais d&#39;identifications anonymes et de visites sur site, l&#39;Adobe traite ces données pour former des groupes de dispositifs qui représentent un groupe de dispositifs utilisés par une personne inconnue. Ces grappes d&#39;appareils sont fournies aux membres de Device Co-op et utilisées pour offrir à leurs consommateurs une meilleure expérience, plus cohérente, entre appareils.

**Comment les périphériques de  [!DNL Device Co-op] liaison fonctionnent-ils ?**

Voir [Liens déterministes et probabilistes](processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931).

**Quelles données les participants fournissent-ils  [!DNL Adobe]?**

Voir [Outil d’exclusion pour les consommateurs, Confidentialité et le graphique de périphériques](privacy.md#concept-fa1346e6b95a484eaeafc9bebe3cd6be).

**Quelles données sont partagées entre  [!DNL Device Co-op] les membres ?**

Voir [Partage de liens dans le graphique de périphériques](processes/link-sharing.md#concept-7168053105a94649a3f092d375d79eaf).

<!--
Removed at Asa's request.
<p><b>What does <span class="keyword"> Adobe </span> see via the <span class="wintitle"> Device Graph </span>?</b> </p>
<p>Adobe can see which devices are most likely being used by the same person, using probabilistic and deterministic device graph algorithms. This match between a group of devices and a person is really two numbers that are linked to each other. One number represents a group of devices believed to belong to the same person while the other number represents a person. Adobe makes this linked device information available to consumers as well, so they can correct misinformation and/or opt-out one or all devices from the Device Co-op. </p>
-->

**Un  [!DNL Device Co-op] membre peut-il voir des liens vers des périphériques qu&#39;il n&#39;a jamais vus auparavant ?**

Non. Les membres Device Co-op peuvent uniquement obtenir des données en fonction des périphériques qui ont consulté l’une des propriétés web de leur marque. Voir [Appareils connus](processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) et [Appareils inconnus](processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40).

**Aurai-je besoin de partager les informations marketing de ma société ?**

Non. Les marques ne fournissent que des données anonymes de périphérique à l’Adobe.

**Utilise-t- [!DNL Adobe] on des informations d’identification personnelle (informations d’identification personnelle) dans  [!DNL Device Co-op]?**

Non. Toutes les informations d’identification personnelle sont hachées avant d’être introduites dans un système d’Adobe, de sorte que les informations de vos clients ne soient jamais transférées vers des systèmes d’Adobe.

**Les petites marques qui apportent moins de données sur les dispositifs à Device Co-op obtiennent-elles plus de valeur que ce qu&#39;elles y investissent, par rapport à leurs homologues plus importants ?**

Non. Tous les membres de la Coopérative obtiennent une valeur de retour par rapport à ce qu&#39;ils y ont mis. Par exemple, si une marque fournit 10 000 périphériques, elle pourra recevoir des informations supplémentaires sur les périphériques liés associées à ces 10 000 périphériques. Dans l&#39;ensemble, cette contribution peut sembler minime ; mais à mesure que de plus en plus de marques de toutes tailles se joignent, la contribution globale est importante et fournira le lien manquant pour de nombreux appareils que de nombreuses autres marques, peut-être plus grandes, recherchent. Voir [Fairness and the Known Device](processes/known-device.md#section-0543188729d845d6b95db70b8b25e9f8).

**Comment  [!DNL Adobe] gérer les adresses IP si certains pays considèrent une adresse IP comme des informations personnelles ?**

La Device Co-op est d&#39;abord diffusée aux États-Unis et au Canada où l&#39;adresse IP n&#39;est pas considérée comme des renseignements personnels. Lorsque la Coopérative est publiée dans les pays où l&#39;adresse IP est considérée comme des renseignements personnels, l&#39;adresse IP ne sera pas utilisée.
