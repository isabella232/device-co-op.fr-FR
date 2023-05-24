---
description: Réponses aux questions courantes sur Device Co-op (Identity Services Cooperation et Identity Graph).
title: FAQ sur Device Co-op
uuid: 490566e1-4d35-468c-8389-678f9ff02cc8
exl-id: 6511e247-76a7-4960-944c-b49fd046fb28
source-git-commit: 399a4fe2d34957eafe8c4eebed465df8770a9239
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# FAQ{#faq}

Descriptions et réponses aux questions courantes sur la coopérative Identity Services et le graphique d’identités.

**Qu’est-ce que la variable [!DNL Device Co-op]?**

Device Co-op est une coopérative numérique qui permet aux clients Adobe Experience Cloud participants de travailler ensemble pour mieux identifier leurs clients sur différents appareils.

**Quelles sont les technologies utilisées dans Device Co-op ?**

Device Co-op se compose de deux technologies :

* **Service d’ID d’Experience Cloud :** Ce service principal de Adobe Experience Cloud fournit un identifiant commun permettant d’identifier les consommateurs de manière cohérente à l’échelle de toutes les solutions, canaux, expériences et périphériques.
* **Adobe Experience Cloud Device Co-op :** Cette technologie relie différents appareils utilisés par un consommateur ou un foyer.

**Comment fonctionne la variable [!DNL Device Co-op] travail ?**

Alors que les marques lancent dans leur pièce du puzzle multi-appareils par le biais de connexions anonymes et de visites sur le site, Adobe traite ces données pour former des grappes de périphériques qui représentent un groupe d’appareils utilisés par une personne inconnue. Ces grappes d’appareils sont données aux membres de Device Co-op et sont utilisées pour offrir à leurs clients une expérience plus cohérente et plus efficace entre appareils.

**Comment fonctionne la variable [!DNL Device Co-op] lier les appareils ?**

Voir [Liaisons déterministes et probabilistes](processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931).

**Quelles données les participants fournissent ? [!DNL Adobe]?**

Voir [Outil d’exclusion pour les consommateurs, confidentialité et Device Graph](privacy.md#concept-fa1346e6b95a484eaeafc9bebe3cd6be).

**Quelles données sont partagées entre [!DNL Device Co-op] membres ?**

Voir [Partage de liens dans Device Graph](processes/link-sharing.md#concept-7168053105a94649a3f092d375d79eaf).

<!--
Removed at Asa's request.
<p><b>What does <span class="keyword"> Adobe </span> see via the <span class="wintitle"> Device Graph </span>?</b> </p>
<p>Adobe can see which devices are most likely being used by the same person, using probabilistic and deterministic device graph algorithms. This match between a group of devices and a person is really two numbers that are linked to each other. One number represents a group of devices believed to belong to the same person while the other number represents a person. Adobe makes this linked device information available to consumers as well, so they can correct misinformation and/or opt-out one or all devices from the Device Co-op. </p>
-->

**Peut [!DNL Device Co-op] Le membre voit des liens vers des appareils qu’il n’a jamais vus auparavant ?**

Non. Les membres de Device Co-op peuvent uniquement obtenir des données en fonction des appareils qui ont visité l’une des propriétés web de leur marque. Voir [Périphériques connus](processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) et [Périphériques inconnus](processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40).

**Devrai-je partager les informations marketing de mon entreprise ?**

Non. Les marques ne fournissent que des données anonymes de périphérique à Adobe.

**Does [!DNL Adobe] utiliser des informations d’identification personnelle dans la variable [!DNL Device Co-op]?**

Non. Toutes les informations d’identification personnelle sont hachées avant d’être introduites dans un système d’Adobe, de sorte que les informations de votre client ne soient jamais transférées vers les systèmes d’Adobe.

**Les marques plus petites qui apportent moins de données sur les appareils à Device Co-op ont-elles plus de valeur que ce qu’elles y investissent, par rapport à leurs homologues plus grandes ?**

Non. Tous les membres de la coopérative obtiennent une valeur de retour par rapport à ce qu&#39;ils y ont mis. Par exemple, si une marque fournit 10 000 appareils, elle pourra recevoir des informations supplémentaires sur les appareils associés à ces 10 000 appareils. Dans l&#39;ensemble, cette contribution peut sembler minime; mais à mesure que de plus en plus de marques de toutes tailles se joignent, la contribution globale est importante et fournira le lien manquant pour de nombreux appareils que de nombreuses autres marques, peut-être plus grandes, recherchent. Voir [Équité et appareil connu](processes/known-device.md#section-0543188729d845d6b95db70b8b25e9f8).

**Comment [!DNL Adobe] gérer les adresses IP si certains pays considèrent une adresse IP comme des informations personnelles ?**

Device Co-op est d’abord disponible aux États-Unis et au Canada, où l’adresse IP n’est pas considérée comme des informations personnelles. Lorsque la coopérative est publiée dans les pays où l’adresse IP est considérée comme des informations personnelles, l’adresse IP ne sera pas utilisée.
