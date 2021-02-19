---
description: A propos du partage de liens dans le graphique de périphériques.
seo-description: A propos du partage de liens dans le graphique de périphériques.
seo-title: Partage de liens dans le graphique de périphériques
title: Partage de liens dans le graphique de périphériques
uuid: 6c7202f0-c6d9-48a4-82ad-ee57d7a518a0
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---


# Partage de liens dans le graphique de périphériques {#link-sharing-in-the-device-graph}

A propos du partage de liens dans le graphique de périphériques.

Le [!DNL Device Graph] partage des liens déterministes et probabilistes avec différents membres de la Adobe Experience Cloud Device Co-op. Le partage de liens est ce qui rend le [!DNL Device Co-op] si puissant. Il étend ce que chaque membre sait des appareils associés à une personne anonyme, mais seulement si vous avez déjà vu au moins un des appareils de cette personne anonyme auparavant.

## Récapitulatif du graphique de périphérique {#section-7858e9f61b5644c981ffb53626fcc19d}

Avant de commencer, examinons le fonctionnement de [!DNL Device Graph]. Les membres de [!DNL Device Co-op] envoient des données à [!DNL Device Graph]. [!DNL Device Graph] utilise ces données pour construire l&#39;identité d&#39;une personne à partir de [liens déterministes et probabilistes](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931) entre les dispositifs. En tant que participant [!DNL Device Co-op], ces liens fournissent des informations sur la relation entre vos utilisateurs authentifiés, d’autres utilisateurs et leurs périphériques. Voyons comment cela fonctionne dans la section ci-dessous.

## Exemple de partage de liens {#section-cb410d827cf14f76bc9b0bd4d31ed767}

L&#39;exemple suivant illustre la puissance du partage de liens dans Device Co-op. Dans cet exemple, nous avons deux sociétés fictives, la Société des actualités et la Société des finances. Les deux sociétés sont membres du [!DNL Device Co-op]. La personne A est un consommateur qui se connecte ou navigue sur les sites Web de chaque société à partir de plusieurs périphériques.

![](assets/share1.png)

Comme la personne A s&#39;est authentifiée sur le site d&#39;informations avec son téléphone portable et sa tablette, la Société d&#39;informations les identifie avec un identifiant de consommateur. Il envoie cet identifiant à [!DNL Device Graph] en tant que hachage cryptographique. La Société des finances a déjà vu ces appareils auparavant, mais la personne A n&#39;a pas ouvert de session sur le site. Par conséquent, la Société des finances ne sait pas si ou comment ces dispositifs se connectent les uns aux autres ni comment ils sont associés à la personne A.

![](assets/share2.png)

Compte tenu du hachage cryptographique de l&#39;ID de consommateur, le [!DNL Device Graph] reconnaît que ces dispositifs sont liés les uns aux autres et à une personne particulière. Pour les sociétés qui ne participent pas à [!DNL Device Co-op] ces visites sur le site semblent provenir de dispositifs aléatoires distincts. Dans tous les cas, une fois que l&#39;identifiant [!DNL Device Graph] a été haché, il est :

* Les téléphones portables et portables connus sont liés.
* Reconnaît que la Société des finances souhaite savoir si le téléphone portable et l&#39;ordinateur portable sont liés.

Dans ces conditions, le [!DNL Device Graph] partage maintenant le lien reliant ces périphériques pour la Société des nouvelles à la Société des finances. Au cours de ce processus, le [!DNL Device Graph] duplicata et partage le lien d&#39;un membre coopératif à un autre.

![](assets/share3.png)

À ce stade, le [!DNL Device Graph] a joué son rôle avec succès. Tant la Société des nouvelles que la Société des finances ont une image claire d&#39;une identité. Ils peuvent atteindre la personne A avec précision sur tous leurs appareils.

## Confidentialité et partage de liens {#section-7b566018b3304420a4b3e4c079826110}

Le maintien de la confidentialité des données et de l&#39;intégrité des données des membres [!DNL Device Co-op] est essentiel tout au long du processus de partage des liens. Au cours de ce processus d&#39;identification des clients et de partage de liens, [!DNL Device Graph] n&#39;a pas :

* Dites à la Société des Finances que le lien provient de la Société des nouvelles.
* Partagez l&#39;ID de client utilisé par un membre [!DNL Device Co-op] avec un autre membre.
* Fournissez toute information autre que celle selon laquelle le périphérique mobile et l&#39;ordinateur portable partagent un lien en commun.

## Étapes suivantes {#section-ac6e61f1eb6e45b1bb4be8ece39147c7}

La lecture de la documentation sur l&#39;identité, les liens et le partage de liens doit vous donner une bonne idée de la façon dont [!DNL Device Graph] assemble les données en interne. À l&#39;étape suivante, nous vous recommandons de jeter un coup d&#39;oeil à notre documentation qui décrit comment le concept d&#39;un *`known device`* fournit des liens inter-périphériques aux membres Device Co-op. Voir [Appareils connus](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) et [Appareils inconnus](../processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40).
