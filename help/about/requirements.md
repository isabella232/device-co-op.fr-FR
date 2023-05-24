---
description: Votre entreprise doit respecter ces normes minimales avant de pouvoir commencer à utiliser Device Co-op Experience Cloud.
seo-description: Your company must meet these minimum standards before you can start using the Experience Cloud Device Co-op.
seo-title: Membership requirements
title: Conditions d’adhésion
uuid: 4295fa4e-1b9e-4323-bb79-48e548ca1167
exl-id: 923ce9c5-7716-4c5a-95f2-05a81a05c9cf
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 17%

---

# Conditions d’adhésion{#membership-requirements}

Votre entreprise doit respecter ces normes minimales avant de pouvoir commencer à utiliser Device Co-op Experience Cloud.

## Conditions requises {#section-9cbcee3c7b4e4c49b4c0e2b26aec5fe9}

Contactez votre [!DNL Adobe representative to get started]. Adobe se réserve le droit de refuser toute appartenance potentielle d’un client à Device Co-op Experience Cloud si l’Adobe détermine que la participation d’un client potentiel à Device Co-op peut (1) enfreindre toute loi en vigueur ; ou (2) présentent un risque matériel pour la sécurité ou les opérations d&#39;Adobe ou de l&#39;un de ses clients.

## Conditions requises pour les Experience Cloud {#section-76218a50385d43e6b9323e49f598394a}

Vous devez activer pour la variable [!DNL Adobe Experience Cloud] et utiliser les solutions et services suivants pour participer à la coopérative.

**Solutions**

Les candidats doivent utiliser au moins l’une des méthodes suivantes : [!DNL Adobe]solutions :

* [Analytics](http://www.adobe.com/fr/marketing-cloud/web-analytics.html)
* [Audience Manager](http://www.adobe.com/fr/marketing-cloud/data-management-platform.html)
* [Adobe Media Optimizer](http://www.adobe.com/marketing-cloud/online-advertising-management.html)
* [Target](http://www.adobe.com/fr/marketing-cloud/testing-targeting.html)

**Services principaux**

Les candidats doivent mettre en oeuvre la variable [Service d’ID Experience Cloud](https://docs.adobe.com/content/help/fr-FR/id-service/using/home.html).

## Configuration requise pour la bibliothèque de code d’Adobe {#section-931a3fca1ce54afd90b88ba032e75f05}

Le tableau suivant répertorie les versions minimales des bibliothèques de code ou des SDK utilisés par diverses [!DNL Experience Cloud] solutions et services. Si vous utilisez l’un de ces codes et souhaitez participer à Device Co-op, assurez-vous de respecter ces exigences minimales.

>[!TIP]
>
>Il est recommandé d’utiliser les versions de code les plus récentes plutôt que les versions minimales requises.

**AppMeasurement (Flash)**

Version 4.1 requise. Voir [AppMeasurement pour Flash, Flex et AIR](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/data-insertion-api/index.md).

**AppMeasurement (JavaScript)**

Version 1.5.4 requise. Voir [AppMeasurement pour Flash, Flex et AIR](https://docs.adobe.com/content/help/fr-FR/analytics/implementation/js/migrate-from-hcode.html).

**SDK mobiles**

Configuration minimale requise pour le SDK mobile :

* Android version 4.8.3.
* iOS version 4.8.5.

Le code de votre SDK doit être activé pour la variable [!DNL Experience Cloud] Service d’ID. Activez et téléchargez le dernier code du SDK pour chaque application de votre [Adobe Mobile Services](https://mobilemarketing.adobe.com/) compte . Voir [Configuration des options du SDK Service d’identification des visiteurs](https://docs.adobe.com/content/help/fr-FR/mobile-services/using/manage-app-settings-ug/configuring-app/t-config-visitor.html).

Pour chaque SDK, utilisez les `visitorSyncIdentifier` selon vos besoins. Voir :

* [Méthodes du service d’ID Experience Cloud Android](https://docs.adobe.com/content/help/en/mobile-services/android/experience-cloud-android/mcvid.html)
* [Méthodes du service d’ID d’Experience Cloud iOS](https://docs.adobe.com/content/help/en/mobile-services/ios/exp-cloud-ios/mcvid.html)

**VisitorAPI.js**

Version 1.5.4 requise.

[!DNL Analytics] Les clients peuvent télécharger la bibliothèque VisitorAPI.js depuis [!DNL Code Manager]. Il se trouve dans les fichiers JavaScript (nouveau) ou JavaScript (hérités). Contact [Assistance clientèle](https://helpx.adobe.com/fr/marketing-cloud/contact-support.html) si vous n’avez pas accès à [!DNL Code Manager].

**Bibliothèque Target**

Nécessite l’une des conditions suivantes : [!DNL Target] Bibliothèques JavaScript :

* at.js (toute version)
* mbox.js version 58 ou ultérieure
