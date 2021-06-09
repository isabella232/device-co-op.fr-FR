---
keywords: adobe experience cloud;Adobe Experience Cloud;device co-op;Device Co-op;fin de vie
solution: Adobe Experience Cloud
title: FAQ sur la fin de vie de Device Co-op
description: Découvrez les plans de fin de vie de Device Co-op.
source-git-commit: b9e21ba2f749b7a4ad69c122e2273b7f3309da58
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 2%

---

# FAQ sur la fin de vie de Device Co-op

Ce document répond aux questions les plus fréquemment posées sur le plan de fin de vie de Adobe Experience Cloud Device Co-op (EOL). Lorsque ce plan entrera en vigueur, Adobe indiquera de manière avancée les [notes de mise à jour de l’Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=fr) et la [mise à jour prioritaire du produit](https://www.adobe.com/subscription/priority-product-update.html).

## FAQ

Vous trouverez ci-dessous une liste de réponses aux questions fréquentes sur le plan de fin de vie.[!DNL Device Co-op]

## Pourquoi [!DNL Device Co-op] est-il obsolète ?

Les changements à venir dans l’environnement d’AdTech devraient entraîner l’obsolescence de [!DNL Device Co-op] dans les années à venir. [!DNL Device Co-op] est principalement constitué de cookies tiers et  [!DNL Google's] d’annonce qu’ils bloqueront les cookies tiers d’ [!DNL Google Chrome] ici 2022 diminuera l’efficacité de  [!DNL Device Co-op]. [!DNL Chrome] représente environ 65 % de la part de marché du navigateur et d’autres navigateurs majeurs ont déjà mis en oeuvre le blocage des cookies tiers. Une fois que [!DNL Chrome] bloque les cookies tiers, la majorité des cookies tiers sont bloqués et [!DNL Device Co-op] devient obsolète.

## Pourquoi les inscriptions à l’Adobe se terminent-elles [!DNL Device Co-op] maintenant ?

Les inscriptions se terminent afin d’éviter les risques de ne pas répondre aux attentes des clients en raison des changements à venir du secteur concernant les cookies tiers. [!DNL Device Co-op] prend quelques mois pour être préparé et quelques autres mois pour extraire de la valeur du service. Si d’autres inscriptions se produisent à ce stade, les marques peuvent ne pas bénéficier pleinement de [!DNL Device Co-op].

## Les nouveaux clients peuvent-ils s’inscrire ?

À compter du 11 juin 2021, Adobe n’acceptera plus les nouvelles inscriptions à [!DNL Device Co-op].

## Les contrats existants sont-ils renouvelés ?

À compter du 11 juin 2021, Adobe ne renouvellera plus les contrats [!DNL Device Co-op]. Si vous souhaitez continuer à utiliser les services [!DNL Device Co-op] , vous pouvez continuer à le faire en vertu des conditions de licence actuelles jusqu’à la fin du programme.

## Quelle est la date exacte de fin du programme [!DNL Device Co-op] ?

Le programme [!DNL Device Co-op] prendra fin en 2022. La date et l’heure spécifiques dépendent du moment où [!DNL Google] commence à bloquer les cookies tiers.

## Quelles applications seront affectées par la fin de vie de Device Co-op ?

Les applications suivantes seront affectées par les procédures de fin de vie de [!DNL Device Co-op] :

- [Adobe Analytics](https://experienceleague.adobe.com/docs/analytics.html?lang=en)
- [Adobe Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/overview/aam-overview.html?lang=en)
- [Adobe Advertising Cloud](https://experienceleague.adobe.com/docs/advertising-cloud.html?lang=en)
- [Adobe Target](https://experienceleague.adobe.com/docs/target/using/introduction/intro.html?lang=en)

## Quelles options ai-je comme alternative à [!DNL Device Co-op] ?

### [!DNL Analytics]

Vous pouvez utiliser la fonction [!DNL Analytics] [Analyses entre appareils (CDA)](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html), car elle prend en charge le service Adobe Experience Platform Identity [Graph privé](https://experienceleague.adobe.com/docs/analytics/components/cda/device-graph.html?lang=en) et le [Assemblage basé sur les champs](https://experienceleague.adobe.com/docs/analytics/components/cda/field-based-stitching.html?lang=en).

### [!DNL Audience Manager]

[!DNL Audience Manager] conserve les intégrations avec des partenaires graphiques d’appareils tiers, y compris  [!DNL LiveRamp] et  [!DNL Tapad], bien que vous deviez établir des relations commerciales avec les partenaires graphiques directement, afin de tirer parti de  [!DNL Audience Manager].

### [!DNL Real-time Customer Data Platform]

Il n’est pas prévu de modifier la [!DNL Audience Manager Data Management Platform] actuelle (DMP). Cependant, l’abandon des cookies tiers va probablement créer des défis d’échelle pour la plupart des utilisateurs DMP. Pour aider les clients à développer leurs pratiques de gestion des données, Adobe encourage la réduction des dépendances sur les identifiants qui seront soumis à des restrictions au cours de l’année à venir. Les équipes marketing doivent élaborer des stratégies de données propriétaires axées sur les identifiants durables qui incluent des informations d’identification personnelle (PII), qui peuvent être résolues avec [!DNL Real-time Customer Data Platform] (CDP en temps réel).

[!DNL Real-time CDP] réduit les dépendances aux cookies tiers et aux identifiants d’appareil en développant l’ensemble d’identifiants disponibles pour la création d’audience afin d’inclure les informations d’identification personnelle. Le composant de base de [!DNL Real-time CDP] est Real-time Customer Profile, qui rassemble en temps réel les données d’attributs de personne avec les données comportementales et permet aux marketeurs de créer des segments d’audience riches avec des contrôles de gouvernance des données brevetés. Comme [!DNL Audience Manager], [!DNL Real-time CDP] fournit des informations et des cas d’utilisation de la personnalisation, mais génère également des informations plus granulaires au niveau de la personne et peut activer les audiences vers un plus large éventail de destinations couvrant les technologies publicitaires et les technologies marketing, y compris les médias payants, les médias sociaux, le courrier électronique et les systèmes clients.

[!DNL Real-time CDP] inclura également l’accès à la correspondance de segment  [Adobe Experience Platform (Alpha)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match.html?lang=en), qui permet aux marques d’étendre leurs propres jeux de données propriétaires par le biais de partenariats et d’obtenir de meilleures informations et une meilleure personnalisation.

### [!DNL Target]

Il n’existe actuellement aucune alternative disponible pour [!DNL Target] car [!DNL Target] offre une fonctionnalité de combinaison d’identités déterministe entre appareils appelée `mbox3rdPartyId`, qui fonctionne de la même manière que l’ID de client de l’Adobe. Cette fonctionnalité permet aux clients [!DNL Target] de fusionner les profils et la participation aux activités dans [!DNL Target] tests et personnalisation effectués dans les canaux entrants.

### Adobe Advertising Cloud

[!DNL Advertising Cloud] les clients ne pourront plus utiliser  [!DNL Device Co-op] pour le ciblage et la mesure d’audiences sur plusieurs appareils. Avec [!DNL Advertising Cloud], vous pourrez continuer à tirer parti du partenariat [!DNL Device Graph] de l’Adobe avec [!DNL LiveRamp] pour continuer à exécuter ces fonctions dans la mesure de la [!DNL LiveRamp’s] capacité et de l’échelle. Vous devez autoriser vos campagnes qui utilisent [!DNL Device Co-op] à se terminer, puis passer au fournisseur de graphiques de périphérique [!DNL LiveRamp] ou ne plus exploiter le ciblage basé sur les personnes.

## Quelles fonctionnalités et mises en oeuvre existantes peuvent m’aider à me préparer à un avenir sans cookie ?

Votre mise en oeuvre du service d’identification des visiteurs existante alimente Analytics [CDA](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html). Si votre ID déclaré existant est un message électronique haché, il peut être utilisé pour alimenter les fonctionnalités suivantes :

- [!DNL Audience Manager] [Destinations basées sur des personnes](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/people-based/people-based-destinations-overview.html).
- [Correspondance de segment Experience Platform (Alpha)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match.html?lang=en).

## Puis-je conserver mes données de [!DNL Device Co-op] ?

Pour les utilisateurs [!DNL Audience Manager] et [!DNL Advertising Cloud], les données de [!DNL Device Co-op] ne seront pas disponibles pour être transférées vers des graphiques tiers. [!DNL Device Co-op] Les données ne seront migrées que pour  [!DNL Analytics Ultimate] les utilisateurs qui utilisent les analyses entre appareils avec le  [!DNL Device Co-op] passage au regroupement basé sur les champs. Les données de toutes les autres solutions ne seront pas migrées.

## Est-il obligatoire d’adopter d’autres caractéristiques ?

Bien que l’adoption d’autres fonctionnalités d’Adobe ne soit pas obligatoire, vous devez commencer à mettre en oeuvre d’autres fonctionnalités dès que possible afin de permettre le temps et une coordination appropriée avant l’obsolescence de [!DNL Device Co-op].

## Quand dois-je adopter des solutions alternatives si je le choisis ?

L&#39;adoption d&#39;autres fonctionnalités n&#39;est pas obligatoire. Il est uniquement recommandé si vous souhaitez continuer à traiter les cas d’utilisation qui ont été traités par [!DNL Device Co-op]. Si vous choisissez d’adopter d’autres fonctionnalités, vous devez le faire d’ici 2022 (calendrier exact à annoncer) avant la fin du programme [!DNL Device Co-op].

## Combien de temps durera l&#39;adoption ?

Cela dépend de la fonctionnalité. Par exemple, si un client Analytics Ultimate qui utilise Analytics sur l’ensemble des appareils avec [!DNL Device Co-op] doit migrer vers Real-time Private Device Graph ou le regroupement basé sur les champs, l’adoption prendra du temps.