---
description: Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.
seo-description: Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.
seo-title: Target - Tests A/B, tests multivariés et ciblage d’expérience
title: Target - Tests A/B, tests multivariés et ciblage d’expérience
uuid: c1b478a4-812e-41ee-913f-29666c5c7ec4
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031

---


# Target - A/B tests, multivariate tests, and experience targeting{#target-a-b-tests-multivariate-tests-and-experience-targeting}

Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.

Vous pouvez utiliser les données Device Co-op dans les tests A/B, les tests multivariés (MVT) et les activités de ciblage d’expérience. The Device Co-op option is available during activity creation on the [!DNL Goals & Settings] page in the [!DNL Target] three-step guided workflow.

Vous ne pouvez pas utiliser les données Device Co-op dans les activités de personnalisation automatisée, de recommandation ni dans celles utilisant [!DNL Adobe Analytics] comme source de rapports (intégration de [!DNL Target] et [!DNL Analytics] appelée A4T).

>[!NOTE]
>
>Ensure that you have the required version of `mbox.js`. Vous pouvez utiliser n’importe quelle version d’`at.js`. Pour plus d’informations, voir Conditions [d’](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43)adhésion.

## Deliver relevant content regardless of the device {#section-bba8d41e96914c82a6d267a54f776354}

Les marketeurs cherchent à présenter à chaque visiteur le contenu le plus pertinent, quel que soit le périphérique que ce dernier utilise pour interagir avec leur entreprise ou leur marque.

Les utilisateurs interagissent avec une même entreprise ou marque depuis divers périphériques : ordinateur portable professionnel, ordinateur personnel, iPad, iPhone, navigateurs variés, etc. Si vous ne pouvez pas reconnaître qu’un périphérique ou navigateur donné est utilisé par la même personne qui a déjà interagi avec votre marque depuis un autre périphérique ou navigateur, vous ne pouvez pas offrir une expérience cohérente et ciblée à cette personne.

Grâce à Device Co-op, ces différents périphériques peuvent être identifiés comme étant utilisés par le même utilisateur. Quand cet utilisateur navigue sur une page avec des activités [!DNL Target] (des activités ou du contenu ciblé), [!DNL Target] peut s’assurer qu’il consulte le même contenu que celui qu’il a consulté sur un autre périphérique.

## Analyze Target activities by people instead of by visitors {#section-c25cf4f8483942d7836d60756235e62c}

Les marketeurs cherchent à analyser les activités de [!DNL Target] par « personnes » plutôt que par « visiteurs ».

Chaque personne est susceptible d’interagir avec une même entreprise ou marque depuis plusieurs périphériques et navigateurs. Toutefois, sans Device Co-op, chaque périphérique ou navigateur est considéré comme un « visiteur » distinct dans les rapports [!DNL Target].

L’affichage des rapports par périphérique et navigateur uniques gonfle considérablement le nombre de « visiteurs » interagissant avec l’entreprise ou la marque. En général, chacune de ces personnes donnera réellement lieu à une seule conversion, même si plusieurs périphériques et navigateurs ont été utilisés. Ainsi, le taux de conversion rapporté sera inférieur au taux réel car plus de « visiteurs » seront comptabilisés pour une seule conversion.

Avec Device Co-op, la diffusion du contenu et la génération de rapports sont axées sur les « personnes », de sorte que les rapports présentent exactement combien de personnes différentes ont vu l’activité et combien ont converti leur activité.

Sans les données de Device Co-op, vous pourriez bien vous féliciter des performances d’une activité qui, en réalité, rapports de Device Co-op à l’appui, n’est pas précisément celle qui a enregistré le taux de conversion le plus élevé.

Pour en savoir plus sur ce concept, reportez-vous au chapitre [Analytics : Mesure](../other-solutions/people.md#concept-8c57cd3904974e078d7fbf84ac9c2d63)Personnes.

## Use Device Co-op data per activity {#section-fb46fae482654023abb1a1e26564db9a}

Les marketeurs ont la possibilité d’utiliser les données de Device Co-op par activité. Toutefois, certaines activités de [!DNL Target] peuvent ne pas être adaptées aux données Device Co-op comme :

* Les contenus destinés aux utilisateurs d’iPad.

   Les utilisateurs qui consultent d’abord un contenu sur un iPad et continueront à voir ce contenu sur leur ordinateur personnel.

* Une offre de taux d’intérêt ciblant un segment très précis de visiteurs.
* Les produits pouvant faire l’objet d’une publicité réservée à une région spécifique (par exemple, une police d’assurance avec certaines restrictions).

Quand les marketeurs créent des audiences dans [!DNL Target], ils sont avertis si une audience n’est pas adaptée aux activités compatibles avec les données Device Co-op. Les audiences adéquates contiennent tous les visiteurs, les nouveaux visiteurs et les visiteurs récurrents.
