---
description: Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.
seo-description: Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.
seo-title: Cible - Tests A/B, tests multivariés et ciblage d’expérience
title: Cible - Tests A/B, tests multivariés et ciblage d’expérience
uuid: c1b478a4-812e-41ee-913f-29666c5c7ec4
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---


# Cible - Tests A/B, tests multivariés et ciblage d’expérience {#target-a-b-tests-multivariate-tests-and-experience-targeting}

Découvrez comment utiliser les données Device Co-op dans les activités Adobe Target.

Vous pouvez utiliser les données Device Co-op dans les tests A/B, les tests multivariés (MVT) et les activités de ciblage d’expérience. L&#39;option Device Co-op est disponible lors de la création de l&#39;activité sur la page [!DNL Goals & Settings] du workflow guidé en trois étapes [!DNL Target].

Vous ne pouvez pas utiliser les données Device Co-op dans les activités Automated Personalization, les activités de recommandation ou les activités en utilisant [!DNL Adobe Analytics] comme source de rapports (intégration [!DNL Target] et [!DNL Analytics], appelée A4T).

>[!NOTE]
>
>Vérifiez que vous disposez de la version requise de `mbox.js`. Vous pouvez utiliser toute version de `at.js`. Pour plus d&#39;informations, voir [Exigences d&#39;adhésion](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43).

## diffuser le contenu approprié quel que soit le périphérique {#section-bba8d41e96914c82a6d267a54f776354} ;

Les marketeurs souhaitent fournir à chaque visiteur l’expérience la plus pertinente, quel que soit le périphérique utilisé par le visiteur pour interagir avec leur société ou marque.

Les utilisateurs interagissent avec la même société ou marque depuis de nombreux périphériques différents : ordinateurs portables de travail, ordinateurs personnels, iPad, iPhone, navigateurs divers, etc. Si vous ne pouvez pas reconnaître que chaque périphérique ou navigateur spécifique est utilisé par la même personne qui a déjà interagi avec votre marque sur un autre périphérique ou navigateur, vous ne pouvez pas fournir une expérience cohérente et ciblée à cette personne.

Grâce à Device Co-op, les divers périphériques d’un utilisateur peuvent être identifiés comme étant utilisés par le même utilisateur. Lorsque cet utilisateur voit une page avec des activités [!DNL Target] (activités ou contenu ciblé), [!DNL Target] peut s&#39;assurer que l&#39;utilisateur voit la même expérience sur un autre périphérique.

## Analyser les activités de Cible par les personnes plutôt que par les visiteurs {#section-c25cf4f8483942d7836d60756235e62c}

Les marketeurs veulent analyser les activités [!DNL Target] par &quot;personnes&quot; plutôt que par &quot;visiteurs&quot;.

Chaque personne interagit probablement avec la même société ou marque sur les appareils et navigateurs, mais sans Device Co-op, chaque périphérique ou navigateur individuel est considéré comme un &quot;visiteur&quot; distinct dans les rapports [!DNL Target].

L’affichage des rapports par périphériques et navigateurs individuels gonfle le nombre de &quot;visiteurs&quot; à un nombre plus élevé que le nombre de personnes différentes interagissant avec la société ou la marque. En règle générale, ces personnes ne convertissent qu’une seule fois sur ces différents périphériques et navigateurs, de sorte que le taux de conversion sera inférieur à ce qu’il est en réalité, car davantage de &quot;visiteurs&quot; seront comptabilisés pour une seule conversion.

Grâce à Device Co-op, la diffusion et le rapports du contenu sont effectués au niveau des &quot;personnes&quot;, de sorte que les rapports indiquent précisément combien de personnes différentes ont vu l&#39;activité et combien de personnes ont converti.

Sans les données Device Co-op, vous pouvez déterminer qu’une activité particulière est gagnante ; toutefois, comme le rapports est plus précis avec Device Co-op, une autre activité pourrait avoir un taux de conversion plus élevé et, par conséquent, être gagnante.

Pour plus d’informations sur ce concept, voir [Analyses : Mesure Personnes ](../other-solutions/people.md#concept-8c57cd3904974e078d7fbf84ac9c2d63).

## Utiliser les données Device Co-op par activité {#section-fb46fae482654023abb1a1e26564db9a}

Les marketeurs peuvent choisir d’utiliser les données Device Co-op par activité. Certaines activités [!DNL Target] peuvent ne pas être appropriées pour les données Device Co-op, telles que :

* Contenu spécifique adapté aux utilisateurs d’un iPad.

   Les utilisateurs qui commencent par vue une expérience sur un iPad continueront à la voir sur leur ordinateur personnel.

* Offre de taux d&#39;intérêt disponible uniquement pour un segment strict de visiteurs.
* Les produits ne peuvent être annoncés que dans un état spécifique (par exemple, une police d&#39;assurance avec des restrictions de licence).

Lorsque les spécialistes du marketing créent des audiences dans [!DNL Target], ils sont avertis si l&#39;audience n&#39;est pas adaptée aux activités activées pour les données Device Co-op. Les audiences appropriées comprennent tous les visiteurs, les nouveaux visiteurs et les visiteurs de retour.
