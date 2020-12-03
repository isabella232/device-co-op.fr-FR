---
description: Lorsqu’une personne possède des périphériques qui ne sont pas utilisés pour interagir avec votre marque, ces périphériques sont appelés périphériques inconnus.
seo-description: Lorsqu’une personne possède des périphériques qui ne sont pas utilisés pour interagir avec votre marque, ces périphériques sont appelés périphériques inconnus.
seo-title: Périphériques inconnus
title: Périphériques inconnus
uuid: 18e69dad-bdb3-4ac1-a690-374aba1aa0a6
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# Périphériques inconnus{#unknown-devices}

Lorsqu’une personne possède des périphériques qui ne sont pas utilisés pour interagir avec votre marque, ces périphériques sont appelés périphériques inconnus.

## Catégories de périphériques inconnues {#section-014b83fd0f2e4d50aa19dd9fbb46f6ab}

Il existe plusieurs façons ou catégories par lesquelles un périphérique peut être considéré comme &quot;inconnu&quot; pour vous. Ces cas comprennent notamment :

* **Visites de premier niveau à d&#39;autres membres de Device Co-op :** Les visites sur d’autres sites [!DNL Device Co-op] membres ou les publicités sur un périphérique ne font pas en elles-mêmes connaître un périphérique à votre marque.

* **Inventaire des publicités non suivi :** Le stock de publicité disponible, mais non encore diffusé ou ingéré, ne fait pas connaître un périphérique à votre marque.
* **Exclusion du consommateur :** Pour respecter le désir des consommateurs, les dispositifs qui ont été désactivés ne sont pas considérés comme des dispositifs connus.

Contrairement aux périphériques connus, les périphériques inconnus ne sont pas liés à d&#39;autres périphériques ou associés à des personnes individuelles.

## Règles de définition de l’état connu/inconnu {#section-fa5c85e59e2d4f88bb79f27f17f02344}

Le [!DNL Device Graph] groupe tente d&#39;être inclusif autant que possible lors de la classification des périphériques connus par rapport à inconnus. Les règles qui permettent de déterminer l’état connu/inconnu fonctionnent dans l’ordre de priorité (1 est le plus élevé) comme indiqué ci-dessous :

* **Règle 1 :** L&#39;appareil est-il désactivé ? Si oui, le périphérique est inconnu.
* **Règle 2 :** L&#39;appareil est-il connu par *une quelconque* méthode ? Si oui, le périphérique est connu.

* **Article 3 : ** Si le précédent ne s&#39;applique pas, l&#39;appareil est inconnu.

>[!MORELIKETHIS]
>
>* [Périphériques connus](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1)

