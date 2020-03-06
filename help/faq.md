---
description: Descriptions et réponses aux questions fréquentes à propos de la coopérative des services d’identité (Identity Services Cooperative) et du graphique des identités (Identity Graph).
seo-description: Descriptions et réponses aux questions fréquentes à propos de la coopérative des services d’identité (Identity Services Cooperative) et du graphique des identités (Identity Graph).
seo-title: FAQ
title: FAQ
uuid: 490566e1-4d35-468c-8389-678f9ff02cc8
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031

---


# FAQ{#faq}

Descriptions et réponses aux questions fréquentes à propos de la coopérative des services d’identité (Identity Services Cooperative) et du graphique des identités (Identity Graph).

**Qu&#39;est-ce que c&#39;est[!DNL Device Co-op]?**

Device Co-op est une coopérative numérique qui permet aux clients Adobe Experience Cloud participants de travailler ensemble pour mieux identifier leurs clients sur tous les périphériques.

**Quelles sont les technologies utilisées dans Device Co-op ?**

Device Co-op repose sur deux technologies :

* **Service d’ID Experience Cloud :** Ce service principal d’Adobe Experience Cloud fournit un ID commun permettant d’identifier les consommateurs de manière cohérente entre les solutions, les canaux, les expériences et les périphériques.
* **Adobe Experience Cloud Device Co-op :** Cette technologie relie différents appareils utilisés par un consommateur ou un ménage.

**Comment ça marche[!DNL Device Co-op]?**

Tandis que les marques placent leurs pièces du puzzle multipériphérique par le biais de connexions et de visites de site rendues anonymes, Adobe traite ces données afin de réconcilier les périphériques utilisés par une personne inconnue. Une fois reconstituées, ces grappes de périphériques sont ensuite transmises aux membres de Device Co-op, qui les utilisent pour offrir à leurs clients une expérience multipériphérique plus qualitative et cohérente.

**Comment fonctionnent les périphériques de[!DNL Device Co-op]liaison ?**

See [Deterministic and Probabilistic Links](processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931).

**Quelles données les participants fournissent-ils[!DNL Adobe]?**

Reportez-vous au chapitre [Outil de désabonnement des clients, protection de la vie privée et Device Graph](privacy.md#concept-fa1346e6b95a484eaeafc9bebe3cd6be).

**Quelles données sont partagées entre[!DNL Device Co-op]les membres ?**

See [Link Sharing in the Device Graph](processes/link-sharing.md#concept-7168053105a94649a3f092d375d79eaf).

<!--
Removed at Asa's request.
<p><b>What does <span class="keyword"> Adobe </span> see via the <span class="wintitle"> Device Graph </span>?</b> </p>
<p>Adobe can see which devices are most likely being used by the same person, using probabilistic and deterministic device graph algorithms. This match between a group of devices and a person is really two numbers that are linked to each other. One number represents a group of devices believed to belong to the same person while the other number represents a person. Adobe makes this linked device information available to consumers as well, so they can correct misinformation and/or opt-out one or all devices from the Device Co-op. </p>
-->

**Un membre de[!DNL Device Co-op]peut-il voir les liaisons vers des périphériques qu’il n’a jamais vus auparavant ?**

Non. Les membres de Device Co-op ont seulement accès aux données de périphériques qui ont visité l’un des sites Web de leur marque. Reportez-vous aux chapitres Périphériques [](processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) connus et Périphériques [](processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40)inconnus.

**Dois-je partager les informations marketing de mon entreprise ?**

Non. Les marques ne fournissent à Adobe que des données anonymes sur les périphériques.

**Utilise-t-[!DNL Adobe]il des informations d’identification personnelle dans le[!DNL Device Co-op]?**

Non. Toutes les données personnelles identifiables (PII) sont hachées avant de parvenir à un système Adobe, de sorte que les informations de vos clients ne sont jamais transmises aux systèmes Adobe.

**Les marques de plus petite envergure qui apportent moins de données sur les périphériques à Device Co-op sont-elles plus rétribuées, en rapport à ce qu’elles apportent, que leurs homologues plus importants ?**

Non. Tous les membres de la coopérative sont rétribués au prorata de leur contribution. Si, par exemple, une marque contribue à hauteur de 10 000 périphériques, elle recevra des informations supplémentaires sur les périphériques associés en rapport avec ces 10 000 périphériques. De prime abord, cette contribution peut sembler infime. Toutefois, tandis que de plus en plus de marques de toutes tailles rejoignent la coopérative, la contribution globale deviendra de plus en plus importante et procurera les liaisons manquantes pour nombre de périphériques que d’autres marques, peut-être plus importantes, recherchent. Voir [Fairness et le périphérique](processes/known-device.md#section-0543188729d845d6b95db70b8b25e9f8)connu.

**Comment[!DNL Adobe]gère-t-elle les adresses IP si certains pays considèrent qu’une adresse IP est une donnée personnelle ?**

Device Co-op n’est pour l’instant proposé qu’aux États-Unis et au Canada où les adresses IP ne sont pas considérées comme des données personnelles. Quand il sera proposé dans des pays où les adresses IP sont considérées comme des données personnelles, celles-ci ne seront alors pas utilisées.
