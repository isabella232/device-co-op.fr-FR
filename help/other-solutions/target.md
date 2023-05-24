---
description: Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.
seo-description: Learn how to use Device Co-op data in Adobe Target activities.
seo-title: Target - A/B tests, multivariate tests, and experience targeting
title: 'Target : tests A/B, tests multivariés et ciblage d’expérience.'
uuid: c1b478a4-812e-41ee-913f-29666c5c7ec4
exl-id: 6e630adf-faff-4fe4-b560-febd59964a5f
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Target : tests A/B, tests multivariés et ciblage d’expérience.{#target-a-b-tests-multivariate-tests-and-experience-targeting}

Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.

Vous pouvez utiliser les données de Device Co-op dans les tests A/B, les tests multivariés (MVT) et les activités de ciblage d’expérience. L’option Device Co-op est disponible lors de la création de l’activité sur la page [!DNL Goals & Settings] dans la [!DNL Target] processus assisté en trois étapes.

Vous ne pouvez pas utiliser les données de Device Co-op dans les activités Automated Personalization, les activités de recommandation ou les activités utilisant [!DNL Adobe Analytics] comme source de création de rapports (le [!DNL Target] et [!DNL Analytics] intégration, appelée A4T).

>[!NOTE]
>
>Assurez-vous que vous disposez de la version requise de `mbox.js`. Vous pouvez utiliser n’importe quelle version de `at.js`. Pour plus d’informations, voir [Conditions d’adhésion](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43).

## Diffuser du contenu pertinent quel que soit l’appareil {#section-bba8d41e96914c82a6d267a54f776354}

Les marketeurs souhaitent offrir à chaque visiteur l’expérience la plus pertinente, quel que soit le périphérique utilisé par le visiteur pour interagir avec sa société ou sa marque.

Les utilisateurs interagissent avec la même entreprise ou marque à partir de nombreux appareils différents : Travaillez sur des ordinateurs portables, des ordinateurs personnels, des iPad, des iPhone, divers navigateurs, etc. Si vous ne pouvez pas reconnaître que chaque appareil ou navigateur spécifique est utilisé par la même personne qui a déjà interagi avec votre marque sur un autre appareil ou navigateur, vous ne pouvez pas lui offrir une expérience cohérente et ciblée.

Avec Device Co-op, les différents appareils d’un utilisateur peuvent être identifiés comme étant utilisés par le même utilisateur. Lorsque l’utilisateur voit une page avec [!DNL Target] activités (activités ou contenu ciblé) [!DNL Target] peut s’assurer que l’utilisateur voit la même expérience sur un autre appareil.

## Analyse des activités Target par personnes plutôt que par visiteurs {#section-c25cf4f8483942d7836d60756235e62c}

Les marketeurs veulent analyser [!DNL Target] activités par &quot;personnes&quot; au lieu de &quot;visiteurs&quot;.

Chaque personne interagit probablement avec la même entreprise ou marque sur différents appareils et navigateurs, mais sans Device Co-op, chaque appareil ou navigateur individuel est considéré comme un &quot;visiteur&quot; distinct dans [!DNL Target] rapports.

L’affichage des rapports par appareils et navigateurs individuels gonfle le nombre de &quot;visiteurs&quot; à un nombre plus élevé que le nombre de personnes différentes interagissant avec l’entreprise ou la marque. En règle générale, ces personnes ne convertissent qu’une seule fois sur ces différents appareils et navigateurs. Le taux de conversion sera donc inférieur à la réalité, car davantage de &quot;visiteurs&quot; seront comptabilisés pour une seule conversion.

Grâce à Device Co-op, la diffusion de contenu et la création de rapports se font au niveau des &quot;personnes&quot;. Les rapports indiquent donc précisément combien de personnes différentes ont vu l’activité et combien de personnes ont effectué une conversion.

Sans les données de Device Co-op, vous pouvez déterminer qu’une activité particulière est gagnante. toutefois, comme la création de rapports est plus précise avec Device Co-op, une autre activité peut avoir un taux de conversion plus élevé et, par conséquent, être la gagnante.

Pour plus d’informations sur ce concept, voir [Analytics : Mesure Personnes](../other-solutions/people.md#concept-8c57cd3904974e078d7fbf84ac9c2d63).

## Utilisation des données Device Co-op par activité {#section-fb46fae482654023abb1a1e26564db9a}

Les marketeurs peuvent choisir d’utiliser les données Device Co-op par activité. Certain [!DNL Target] Les activités peuvent ne pas convenir aux données de Device Co-op, telles que :

* Contenu spécifique adapté aux utilisateurs d’une iPad.

   Les utilisateurs qui consultent une expérience pour la première fois sur un iPad continueront à la voir sur leurs ordinateurs personnels.

* Une offre de taux d’intérêt disponible uniquement pour un segment strict de visiteurs.
* Les produits ne peuvent être annoncés que dans un état spécifique (par exemple, une police d’assurance avec des restrictions de licence).

Lorsque les marketeurs créent des audiences dans [!DNL Target], ils sont avertis si l’audience n’est pas adaptée aux activités activées pour les données de Device Co-op. Les audiences appropriées comprennent tous les visiteurs, les nouveaux visiteurs et les visiteurs récurrents.
