---
description: Lorsqu’une personne possède des appareils qui ne sont pas utilisés pour interagir avec votre marque, ces appareils sont appelés appareils inconnus.
seo-description: When a person has devices that are not used to interact with your brand, those devices are called unknown devices.
seo-title: Unknown devices
title: Périphériques inconnus
uuid: 18e69dad-bdb3-4ac1-a690-374aba1aa0a6
exl-id: 7841bf32-7327-4981-86a2-600e2bfe5901
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Périphériques inconnus{#unknown-devices}

Lorsqu’une personne possède des appareils qui ne sont pas utilisés pour interagir avec votre marque, ces appareils sont appelés appareils inconnus.

## Catégories d’appareils inconnues {#section-014b83fd0f2e4d50aa19dd9fbb46f6ab}

Il existe plusieurs façons ou catégories pour qu’un appareil soit considéré comme &quot;inconnu&quot;. Ces cas comprennent notamment :

* **Visites propriétaires vers d’autres membres de Device Co-op :** Visites vers d’autres [!DNL Device Co-op] les sites membres ou la publicité pour un appareil ne font pas en soi connaître un appareil à votre marque.

* **Inventaire d’annonces non suivies :** L’inventaire publicitaire disponible, mais pas encore fourni ou ingéré, ne fait pas connaître un appareil à votre marque.
* **Exclusion des consommateurs :** Pour respecter le désir des consommateurs, les appareils qui ont été désinscrits ne sont pas considérés comme des appareils connus.

Contrairement aux appareils connus, les appareils inconnus ne sont pas liés à d’autres appareils ni associés à des personnes individuelles.

## Règles de définition de l’état connu/inconnu {#section-fa5c85e59e2d4f88bb79f27f17f02344}

Le [!DNL Device Graph] tente d’être le plus inclusif possible lors de la classification des périphériques connus par rapport à inconnus. Les règles qui permettent de déterminer l’état connu/inconnu fonctionnent par ordre de priorité (1 est le plus élevé), comme illustré ci-dessous :

* **Règle 1 :** L’appareil est-il désabonné ? Si oui, l’appareil est inconnu.
* **Règle 2 :** L’appareil est-il connu par *any* méthode ? Si oui, l’appareil est connu.

* **Règle 3 : ** Si la précédente ne s’applique pas, l’appareil est inconnu.

>[!MORELIKETHIS]
>
>* [Périphériques connus](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1)

