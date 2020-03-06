---
description: Les périphériques qu’une personne n’utilise pas pour interagir avec votre marque sont des périphériques inconnus.
seo-description: Les périphériques qu’une personne n’utilise pas pour interagir avec votre marque sont des périphériques inconnus.
seo-title: Périphériques inconnus
title: Périphériques inconnus
uuid: 18e69dad-bdb3-4ac1-a690-374aba1aa0a6
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371

---


# Unknown devices{#unknown-devices}

Les périphériques qu’une personne n’utilise pas pour interagir avec votre marque sont des périphériques inconnus.

## Unknown device categories {#section-014b83fd0f2e4d50aa19dd9fbb46f6ab}

Il existe plusieurs méthodes ou catégories selon lesquelles un périphérique peut être considéré comme « inconnu ». Notamment : 

* **Visites internes sur les sites d’autres membres de  :** les visites sur les sites d’autres membres de [!DNL Device Co-op]Device Co-op ou la publicité sur un périphérique ne suffisent pas, en soi, pour qu’un périphérique soit reconnu par votre marque.

* **Inventaire de publicités non suivies :** l’inventaire de publicités disponibles, mais pas encore diffusées ou ingérées, ne permet pas à votre marque de reconnaître un périphérique.
* **Désabonnement d’un client :** afin de respecter le souhait d’un client, les périphériques désabonnés ne sont pas considérés comme des périphériques connus.

Contrairement aux périphériques connus, les périphériques inconnus ne sont pas liés à d’autres périphériques ni associés à une personne donnée.

## Rules for setting known/unknown status {#section-fa5c85e59e2d4f88bb79f27f17f02344}

Lorsqu’il classifie et distingue les périphériques connus et inconnus, [!DNL Device Graph] tente d’être aussi exhaustif que possible. Les règles qui permettent de les distinguer s’appliquent par ordre de priorité, comme suit :

* **Règle 1 :** le périphérique est-il désabonné ? Dans l’affirmative, le périphérique est inconnu.
* **Règle 2 :** le périphérique est-il connu par *une autre* méthode, quelle qu’elle soit ? Dans l’affirmative, le périphérique est connu.

* **Règle 3 : ** Si le précédent ne s&#39;applique pas, le périphérique est inconnu.

>[!MORELIKETHIS]
>
>* [Périphériques connus](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1)

