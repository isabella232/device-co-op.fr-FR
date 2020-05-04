---
description: La mesure Personnes correspond au nombre de personnes (ou groupes de périphériques) en fonction du graphique de périphériques d’Adobe. Vous pouvez appliquer la mesure Personnes pour identifier les visiteurs sur leurs appareils dans Analyse Workspace.
seo-description: La mesure Personnes correspond au nombre de personnes (ou groupes de périphériques) en fonction du graphique de périphériques d’Adobe. Vous pouvez appliquer la mesure Personnes pour identifier les visiteurs sur leurs appareils dans Analyse Workspace.
seo-title: Mesure Personnes
title: Mesure Personnes
uuid: 8e731779-044d-4d31-a19a-f579a9c8c471
translation-type: tm+mt
source-git-commit: 822882d4f9bb9eed7cf116597b62d07bbe94376c

---


# Mesure Personnes{#people-metric}

La mesure Personnes correspond au nombre de personnes (ou groupes de périphériques) en fonction du graphique de périphériques d’Adobe. Vous pouvez appliquer la mesure Personnes pour identifier les visiteurs sur leurs appareils dans Analyse Workspace.

## Conditions préalables et considérations relatives aux mesures des personnes {#section-34551d0435fb4b3cb3fad736b7961541}

<table id="table_120F7EF50042485391E58B22DD00A2A8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Condition préalable ou considération </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Device Co-op </p> </td> 
   <td colname="col2"> <p> Pour utiliser la mesure Personnes, devenez membre d’ <a href="http://landing.adobe.com/en/na/events/summit/275658-summit-co-op.html" format="html" scope="external"> Adobe Experience Cloud Device Co-op</a>. La coopération identifie plusieurs périphériques (ou identifiants Experience Cloud) d’une personne. Analytics utilise ces informations pour calculer statistiquement le nombre de personnes qui interagissent avec une marque. La mesure est précise à moins de 5 %. </p> <p><b>Régions</b>: La Device Co-op est actuellement disponible uniquement aux États-Unis et au Canada. Par conséquent, lors de l’évaluation de la mesure Personnes, vous devez appliquer à votre analyse un segment qui filtres vos données pour les États-Unis et le Canada uniquement. </p> <p>Chaque semaine, le graphique de périphériques calcule une nouvelle version de la coopérative et la publie en vue de son utilisation. Le mardi, le système collecte les dernières données et publie une version mise à jour du graphique. Les solutions Experience Cloud utilisent ensuite la dernière version du graphique. Dans Analytics, en particulier, les modifications sont lues le mercredi et le traitement des modifications prend généralement entre 1 et 2 jours ouvrés. </p> <p> <p>Important :  Lorsque le graphique se met à jour sur une base hebdomadaire, il peut avoir un impact historique sur la mesure Personnes. En d’autres termes, le décompte historique des personnes peut changer au fil du temps à mesure que le graphique apprend et est mis à jour. Par exemple, si vous exécutez un rapport qui comptabilise les personnes le mois dernier, puis le même rapport une semaine après la mise à jour du graphique, le nombre historique de personnes peut légèrement changer. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Autorisations de mesure </td> 
   <td colname="col2"> <p>Vous ne pouvez utiliser la mesure Personnes que si vous y avez accès. Les administrateurs peuvent<a href="https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/customize-report-access/groups-metrics.html" format="html" scope="external"> personnaliser les autorisations</a> de mesures dans les outils d’administration. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Mappage à l’organisation IMS </td> 
   <td colname="col2"> <p>La mesure Personnes sera activée pour toutes les suites de rapports <a href="https://docs.adobe.com/content/help/fr-FR/core-services/interface/about-core-services/report-suite-mapping.html" format="html" scope="external"> mises en correspondance avec un IMSORG</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Projets/outils d’Analyse </p> </td> 
   <td colname="col2"> <p>Utilisez la mesure Personnes dans <span class="wintitle"> Analyse Workspace</span>, dans une Analyse <span class="wintitle"></span>ad hoc, dans le créateur <span class="wintitle"></span>de rapports et au moyen de l’API. Vous pouvez l’utiliser partout où vous utiliseriez la mesure Visiteurs uniques, y compris les mesures calculées. </p> <p>Par exemple, créez une mesure des recettes par personne pour remplacer une mesure des recettes par visiteur unique. </p> <p>Un modèle <a href="https://docs.adobe.com/content/help/fr-FR/analytics/analyze/analysis-workspace/build-workspace-project/starter-projects.html" format="html" scope="external"> de projet</a> Personnes est disponible pour commencer à utiliser la mesure Personnes dans Analyse Workspace. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activer les règles de robots </p> </td> 
   <td colname="col2"> <p>Adobe recommande d’activer les règles <a href="https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/bot-removal/bot-rules.html" format="html" scope="external"> de</a>robots, en particulier lors de l’utilisation de la mesure Personnes. </p> <p>Lorsqu’un robot analyse votre site Web, il augmente artificiellement le nombre de Visiteurs uniques. La suppression du trafic de robots de votre suite de rapports permet de mesurer plus précisément l’activité de vos propriétés numériques, en termes de Visiteurs uniques et de personnes. </p> <p>Pour ce faire, accédez à <span class="uicontrol"> Analytics</span> &gt; <span class="uicontrol"> Admin</span> &gt; <span class="uicontrol"> Report Suites</span>. Select the correct report suite, and then go to <span class="uicontrol"> Edit Settings</span> &gt; <span class="uicontrol"> General</span> &gt; <span class="uicontrol"> Bot Rules</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Considérations relatives à la segmentation </p> </td> 
   <td colname="col2"> <p> Lorsque vous utilisez des segments avec la mesure Personnes, le rapports de mesures peut être nettement inférieur à ce qui était prévu. </p> <p>Voir <a href="../other-solutions/people.md#section-d03525420dbe48379fd95b230ef05885" format="dita" scope="local"> Utilisation de la mesure Personnes avec des segments</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Qu’est-ce que la mesure Personnes ? {#section-89e2b8f5e80f480391449fc8d1117a6a}

La mesure Personnes est une mesure de rapports Analytics qui vous permet d’attribuer des périphériques à des personnes. Il fournit une vue de marketing basée sur les personnes, vous permettant de mesurer l&#39;activité des visiteurs sur tous leurs appareils. Considérez-le comme une version dédupliquée de Visiteurs uniques et vous pouvez utiliser la mesure Personnes pour l’analyse dans laquelle vous utilisiez auparavant les Visiteurs uniques.

**Les périphériques sont des personnes**

Avant que la mesure Personnes ne soit disponible, une personne (par exemple) peut visiter votre site et interagir avec une campagne ou une marque sur trois périphériques différents et effectuer un achat, même en quelques minutes. Selon votre mise en oeuvre, Analytics peut signaler chaque périphérique comme un visiteur unique et attribuer 10 $ à trois périphériques lors d’un achat de 30 $.

La mesure Personnes vous permet d’attribuer précisément cet achat de 30 euros à une personne :

![](assets/people-centric-results.png)

**Exactitude accrue des rapports**

La mesure Personnes vous permet de considérer plusieurs périphériques comme une seule entité. Le projet Analyse Workspace suivant montre des comparaisons de précision accrues entre le rapports Visiteur unique et le rapports Personnes :

![](assets/people_report.png)

Comparer les personnes et les Visiteurs uniques côte à côte :

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
   <td colname="col1"> <p>Personnes </p> </td> 
   <td colname="col2"> <p>La mesure Personnes repose sur l’idée que les consommateurs interagissent avec votre marque à l’aide de plusieurs périphériques. Plus vous découpez ou segmentez vos données, plus la probabilité qu’une même personne utilise plusieurs périphériques au sein de cette tranche de données est faible. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Visiteurs uniques </p> </td> 
   <td colname="col2"> <p>Par exemple, plus vous répartissez les données par date ou heure, plus la différence entre les personnes et les visiteurs uniques est faible. Si vous souhaitez une bonne compréhension de l’impact global de Device Co-op, Adobe conseille d’utiliser une plage de dates des 90 derniers jours. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Compression </p> </td> 
   <td colname="col2"> <p>A l’aide d’une mesure calculée simple, vous pouvez voir à quel point la mesure Personnes est plus petite qu’un pourcentage de Visiteurs uniques. Cliquez sur l'icône d'information en regard de "Compression" dans le tableau ci-dessus pour voir comment créer cette mesure. </p> <p>Les personnes peuvent être utilisées dans d’autres mesures calculées à la place des Visiteurs uniques. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Comment la mesure Personnes est-elle calculée ? {#section-0dfb762867e14a7f927796ef3c50592b}

<!--
<p>Analytics uses the HyperLogLog statistical algorithm to calculate People. This means that the smaller the data set, the margin for error may increase. No more than 5% of the numbers should be off by more than 5% </p>
-->

L’image suivante montre comment la mesure Personnes est calculée et comment elle peut diminuer au fil du temps au cours de la même période de rapport dans le passé.

![](assets/people-calculations.png)

Dans cet exemple, supposons qu’il existe un ensemble fixe de visiteurs. Si vous exécutez un rapport pour une période fixe dans le passé, il affiche un ensemble fixe de visiteurs. Si le graphique de périphérique génère les données affichées sur le graphique de gauche au cours de la semaine 1, cela représente 90 personnes. Une semaine plus tard, après la prochaine exécution du graphique de périphériques, de nouvelles informations sont prises en compte. Si vous exécutez le même rapport qu&#39;il y a une semaine, le nombre de personnes est descendu à 84. L&#39;historique a changé car le graphique de périphériques fournit de nouvelles informations sur les périphériques à regrouper.

## Utilisation de la mesure Personnes avec des segments {#section-d03525420dbe48379fd95b230ef05885}

Lorsque vous utilisez des segments avec la mesure Personnes, les résultats de la mesure peuvent être nettement inférieurs aux prévisions. Ce problème survient car, dans la segmentation, il n’y a aucun *`person`* conteneur. La segmentation utilise le conteneur du Visiteur, qui est le conteneur de niveau supérieur dans la définition et est basé sur le périphérique, et non sur la personne.

Ce problème survient principalement lors de l’empilement de segments avec la mesure Personnes.

![](assets/people-stacked-segments.png)

L’empilement de segments crée un nouveau segment qui représente la combinaison des segments. L’empilement de segments survient lorsque vous :

* Placez un segment au-dessus d’un autre segment dans l’espace de travail des Analyses. (Ils sont automatiquement joints à l’aide de l’ *`And`* opérateur.)
* Appliquez un segment unique contenant l’ *`And`* opérateur.
* Appliquez un segment au niveau du projet et au niveau du tableau.
* Utilisez une suite de rapports virtuelle avec un autre segment.

Supposons, par exemple, que vous empiliez les segments suivants sur la mesure Personnes :

* `Campaign = Spring Promotion`
* `Site Section = Product Overview`

Seul le nombre de personnes qui remplissent les critères des deux segments *`using a single device`* est comptabilisé. (La mesure Personnes n’affiche pas le nombre de personnes admissibles sur l’ensemble des périphériques.)

En outre, l’utilisation de l’ *`Or`* opérateur n’est pas recommandée dans ce cas. Cela permettrait de calculer le nombre de personnes qui ont vu l&#39;une ou l&#39;autre, sans compter le nombre de personnes admissibles pour les deux segments.

Voir [Création de segments](https://docs.adobe.com/content/help/fr-FR/analytics/components/segmentation/segmentation-workflow/seg-build.html) dans l’aide Segmentation pour plus d’informations.

## Types de périphérique {#section-8ab378c84ff34574b9c20fecb3848a86}

Les mesures Device Co-op et People fonctionnent mieux dans Adobe Analytics lorsque votre suite de rapports contient des données provenant de plusieurs types d’appareils. Par exemple, la combinaison des données web et app dans la même suite de rapports rend la mesure Personnes plus puissante et efficace. Plus vos données comportent de croisement de dispositifs, plus il y a de chances que plusieurs visiteurs uniques soient regroupés en une seule personne.

![](assets/people-device-types.png)

## Experience Cloud ID Service Coverage {#section-bbf0098cac2e467289e7a644a1dea05c}

Device Co-op exige que vos propriétés numériques soient instrumentées à l’aide du service Experience Cloud ID (MCID). Si les données de votre suite de rapports contiennent un nombre important de visiteurs sans MCID, l’efficacité de Device Co-op et de la mesure Personnes est diminuée.

<!--
mcdc-people-metric-apply.xml
-->

Dans Analyse Workspace, créez un [projet](https://docs.adobe.com/content/help/en/analytics/analyze/analysis-workspace/build-workspace-project/t-freeform-project.html), puis faites glisser la **[!UICONTROL People]** mesure vers le tableau du projet :

![](assets/people-metric.png)

