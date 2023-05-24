---
description: La mesure Personnes correspond au nombre de personnes (ou groupes d’appareils) en fonction du graphique de périphérique de l’Adobe. Vous pouvez appliquer la mesure Personnes pour identifier les visiteurs sur leurs appareils dans Analysis Workspace.
seo-description: The People metric is the count of people (or groups of devices) based on Adobe's Device Graph. You can apply the People metric to identify visitors across their devices in Analysis Workspace.
seo-title: People metric
title: Mesure Personnes.
uuid: 8e731779-044d-4d31-a19a-f579a9c8c471
exl-id: e2e70461-19ab-49db-bd65-a3eb26c2d4a8
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 4%

---

# Mesure Personnes.{#people-metric}

La mesure Personnes correspond au nombre de personnes (ou groupes d’appareils) en fonction du graphique de périphérique de l’Adobe. Vous pouvez appliquer la mesure Personnes pour identifier les visiteurs sur leurs appareils dans Analysis Workspace.

## Conditions préalables et considérations relatives aux mesures Personnes {#section-34551d0435fb4b3cb3fad736b7961541}

<table id="table_120F7EF50042485391E58B22DD00A2A8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Condition préalable ou réflexion </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Appareil Co-op </p> </td> 
   <td colname="col2"> <p> Pour utiliser la mesure Personnes, devenez membre du <a href="http://landing.adobe.com/en/na/events/summit/275658-summit-co-op.html" format="html" scope="external"> Adobe Experience Cloud Device Co-op</a>. La coopérative Co-op identifie les multiples appareils (ou identifiants Experience Cloud) d’une personne. Analytics tire parti de ces informations pour dériver statistiquement le nombre de personnes qui interagissent avec une marque. La mesure est précise à moins de 5 %. </p> <p><b>Régions</b>: Device Co-op n’est actuellement disponible qu’aux États-Unis et au Canada. Par conséquent, lors de l’évaluation de la mesure Personnes, vous devez appliquer un segment à votre analyse qui filtre vos données pour les États-Unis et le Canada uniquement. </p> <p>Chaque semaine, Device Graph calcule une nouvelle version de la coopérative et la publie pour utilisation. Le mardi, le système collecte les dernières données et publie une version mise à jour du graphique. Les solutions Experience Cloud utilisent alors la dernière version du graphique. Plus précisément pour Analytics, les modifications sont lues le mercredi et le traitement des modifications prend généralement entre 1 et 2 jours ouvrables. </p> <p> <p>Important : Lorsque le graphique se met à jour chaque semaine, il peut avoir un impact historique sur la mesure Personnes. En d’autres termes, le nombre de personnes historiques peut changer au fil du temps à mesure que le graphique apprend et est mis à jour. Par exemple, si vous exécutez un rapport qui comptabilise les personnes le mois dernier, puis que vous exécutez le même rapport une semaine après la mise à jour du graphique, le nombre historique de personnes peut légèrement changer. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Autorisations de mesure </td> 
   <td colname="col2"> <p>Vous ne pouvez utiliser la mesure Personnes que si vous y avez accès. Les administrateurs peuvent<a href="https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/customize-report-access/groups-metrics.html" format="html" scope="external"> personnalisation des autorisations des mesures</a> dans les outils d’administration. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Mappage à l’organisation IMS </td> 
   <td colname="col2"> <p>La mesure Personnes sera activée pour toutes les suites de rapports qui sont <a href="https://docs.adobe.com/content/help/fr-FR/core-services/interface/about-core-services/report-suite-mapping.html" format="html" scope="external"> mappé à un IMSORG</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Projets/outils d’analyse </p> </td> 
   <td colname="col2"> <p>Utilisez la mesure Personnes dans <span class="wintitle"> Analysis Workspace</span>, <span class="wintitle"> Ad Hoc Analysis</span>, <span class="wintitle"> Report Builder</span>et via l’API. Vous pouvez l’utiliser partout où vous utiliseriez la mesure Visiteurs uniques, y compris les mesures calculées. </p> <p>Par exemple, créez une mesure de recettes par personne pour remplacer une mesure de recettes par visiteur unique. </p> <p>A <a href="https://docs.adobe.com/content/help/fr-FR/analytics/analyze/analysis-workspace/build-workspace-project/starter-projects.html" format="html" scope="external"> Modèle de projet Personnes</a> est disponible pour commencer à utiliser la mesure Personnes dans Analysis Workspace. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activer les règles de robots </p> </td> 
   <td colname="col2"> <p>Adobe recommande d’activer <a href="https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/bot-removal/bot-rules.html" format="html" scope="external"> Règles de robots</a>, en particulier lors de l’utilisation de la mesure Personnes. </p> <p>Lorsqu’un robot analyse votre site web, il augmente artificiellement le nombre de visiteurs uniques. La suppression du trafic de robots de votre suite de rapports permet une mesure plus précise de l’activité sur vos propriétés numériques, à la fois en termes de visiteurs uniques et de personnes. </p> <p>Pour ce faire, accédez à <span class="uicontrol"> Analytics</span> &gt; <span class="uicontrol"> Administration</span> &gt; <span class="uicontrol"> Suites de rapports</span>. Sélectionnez la suite de rapports appropriée, puis accédez à <span class="uicontrol"> Modifier les paramètres</span> &gt; <span class="uicontrol"> Général</span> &gt; <span class="uicontrol"> Règles de robots</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Considérations relatives à la segmentation </p> </td> 
   <td colname="col2"> <p> Lorsque vous utilisez des segments avec la mesure Personnes, les rapports de mesures peuvent être considérablement inférieurs aux prévisions. </p> <p>Voir <a href="../other-solutions/people.md#section-d03525420dbe48379fd95b230ef05885" format="dita" scope="local"> Utilisation de la mesure Personnes avec des segments</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Qu’est-ce que la mesure Personnes ? {#section-89e2b8f5e80f480391449fc8d1117a6a}

La mesure Personnes est une mesure de création de rapports Analytics qui vous permet d’attribuer des périphériques aux personnes. Il offre une vue basée sur les personnes du marketing, ce qui vous permet de mesurer l’activité des visiteurs sur tous leurs appareils. Considérez-le comme une version dédupliquée de Visiteurs uniques et vous pouvez utiliser la mesure Personnes pour l’analyse dans laquelle vous utilisiez auparavant la mesure Visiteurs uniques.

**Les périphériques sont des personnes**

Avant que la mesure Personnes ne soit disponible, une personne (par exemple) peut visiter votre site et interagir avec une campagne ou une marque sur trois appareils différents, puis effectuer un achat, même en quelques minutes. Selon votre mise en oeuvre, Analytics peut signaler chaque appareil comme un visiteur unique et attribuer 10 € à trois appareils pour un achat de 30 €.

La mesure Personnes vous permet d’attribuer précisément cet achat de 30 $ à une personne :

![](assets/people-centric-results.png)

**Précision accrue dans les rapports**

La mesure Personnes vous permet de considérer plusieurs périphériques comme une seule entité. Le projet Analysis Workspace suivant montre des comparaisons plus précises entre les rapports Visiteurs uniques et Personnes :

![](assets/people_report.png)

Comparaison côte à côte des personnes et des visiteurs uniques :

![](assets/people-report.png)

**Définitions**

<table id="table_F8171AF15DA64607B427E3739EF004D6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Élément </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>People </p> </td> 
   <td colname="col2"> <p>La mesure Personnes repose sur l’idée que les consommateurs interagissent avec votre marque à l’aide de plusieurs appareils. Plus vous découpez ou segmentez vos données, plus faible est le risque qu’une même personne ait utilisé plusieurs périphériques au sein de cette tranche de données. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Visiteurs uniques </p> </td> 
   <td colname="col2"> <p>Par exemple, plus vous triez les données par date ou heure, plus la différence entre les personnes et les visiteurs uniques est faible. Si vous souhaitez une bonne compréhension de l’impact global de Device Co-op, Adobe recommande d’utiliser une plage de dates des 90 derniers jours. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Compression </p> </td> 
   <td colname="col2"> <p>Une mesure calculée simple vous permet de voir à quel point la mesure Personnes est plus petite qu’un pourcentage de visiteurs uniques. Cliquez sur l’icône d’information en regard de "Compression" dans le tableau ci-dessus pour voir comment créer cette mesure. </p> <p>Les personnes peuvent être utilisées dans d’autres mesures calculées à la place de Visiteurs uniques. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Comment la mesure Personnes est-elle calculée ? {#section-0dfb762867e14a7f927796ef3c50592b}

<!--
<p>Analytics uses the HyperLogLog statistical algorithm to calculate People. This means that the smaller the data set, the margin for error may increase. No more than 5% of the numbers should be off by more than 5% </p>
-->

L’image suivante montre comment la mesure Personnes est calculée et comment elle peut diminuer au fil du temps pour la même période de rapport dans le passé.

![](assets/people-calculations.png)

Dans cet exemple, supposons qu’il existe un ensemble fixe de visiteurs. Si vous exécutez un rapport pour une période fixe dans le passé, il affiche un ensemble fixe de visiteurs. Si Device Graph génère les données affichées sur le graphique de gauche au cours de la semaine 1, 90 personnes seront alors concernées. Une semaine plus tard, après la prochaine exécution de Device Graph, de nouvelles informations sont prises en compte. Si vous exécutez le même rapport qu&#39;il y a une semaine, le nombre de personnes est descendu à 84. L’historique a changé, car Device Graph fournit de nouvelles informations sur les périphériques à regrouper.

## Utilisation de la mesure Personnes avec des segments {#section-d03525420dbe48379fd95b230ef05885}

Lorsque vous utilisez des segments avec la mesure Personnes, les résultats de la mesure peuvent être considérablement inférieurs aux prévisions. Ce problème se produit car, dans la segmentation, il n’y a pas de *`person`* conteneur. La segmentation utilise le conteneur de visiteurs, qui est le conteneur de niveau supérieur dans la définition et qui est basé sur l’appareil, et non sur la personne.

Ce problème survient principalement lors de l’empilement de segments avec la mesure Personnes.

![](assets/people-stacked-segments.png)

L’empilement de segments crée un segment qui représente la combinaison des segments. L’empilement des segments se produit lorsque vous :

* Placez un segment au-dessus d’un autre segment dans Analysis Workspace. (Ils sont automatiquement unis à l’aide de la fonction *`And`* ).
* Appliquez un seul segment qui contient le *`And`* de l’opérateur.
* Appliquez un segment aux niveaux du projet et du tableau.
* Utilisez une suite de rapports virtuelle avec un autre segment.

Supposons, par exemple, que vous empiliez les segments suivants sur la mesure Personnes :

* `Campaign = Spring Promotion`
* `Site Section = Product Overview`

Uniquement le nombre de personnes qui remplissent les critères dans les deux segments *`using a single device`* sont comptabilisées. (La mesure Personnes n’affiche pas le nombre de personnes admissibles sur l’ensemble des appareils.)

En outre, l’utilisation de la variable *`Or`* n’est pas recommandé dans ce cas. Cela entraînerait le décompte des personnes qui ont vu l’une ou l’autre, sans moyen de compter le nombre de personnes qualifiées pour les deux segments.

Voir [Création de segments](https://docs.adobe.com/content/help/fr-FR/analytics/components/segmentation/segmentation-workflow/seg-build.html) dans l’aide Segmentation pour plus d’informations.

## Types de périphérique {#section-8ab378c84ff34574b9c20fecb3848a86}

La mesure Device Co-op et Personnes fonctionne mieux dans Adobe Analytics lorsque votre suite de rapports contient des données provenant de plusieurs types d’appareils. Par exemple, la combinaison des données web et d’application dans la même suite de rapports rend la mesure Personnes plus puissante et plus efficace. Plus vos données contiennent de périphériques, plus il y a de chances que plusieurs visiteurs uniques soient regroupés en une seule personne.

![](assets/people-device-types.png)

## Couverture du service d’ID Experience Cloud {#section-bbf0098cac2e467289e7a644a1dea05c}

Device Co-op nécessite que vos propriétés numériques soient instrumentées à l’aide du service d’ID Experience Cloud (MCID). Si les données de votre suite de rapports contiennent un nombre important de visiteurs sans MCID, l’efficacité de Device Co-op et de la mesure Personnes est réduite.

<!--
mcdc-people-metric-apply.xml
-->

Dans Analysis Workspace, créez une [project](https://docs.adobe.com/content/help/fr-FR/analytics/analyze/analysis-workspace/build-workspace-project/t-freeform-project.html), puis faites glisser le **[!UICONTROL People]** mesure dans le tableau du projet :

![](assets/people-metric.png)
