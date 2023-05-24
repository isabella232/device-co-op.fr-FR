---
description: Adobe Experience Cloud Device Co-op est un programme qui permet aux participants de travailler ensemble pour mieux identifier les consommateurs à travers les points de contact numériques tout en assurant le niveau de confidentialité et de transparence le plus élevé. Device Co-op Experience Cloud permet aux marques participantes de reconnaître leurs clients afin de leur offrir des expériences plus personnalisées sur tous les appareils et applications, à grande échelle. Device Co-op est un service principal de Adobe Experience Cloud. Il est disponible pour les clients Adobe qui utilisent Analytics, Audience Manager, Media Optimizer ou Target.
seo-description: The Adobe Experience Cloud Device Co-op is a program that lets participants work together to better identify consumers across digital touch points while ensuring the highest level of privacy and transparency. The Experience Cloud Device Co-op empowers participating brands to recognize their consumers so they can deliver more personalized experiences across devices and apps at massive scale. The Device Co-op is a core service of the Adobe Experience Cloud. It is available to Adobe customers who use Analytics, Audience Manager, Media Optimizer, or Target.
seo-title: Overview
title: Aperçu
uuid: 9e2502db-0dc6-4b0f-965f-71894fb1f9d4
exl-id: 8195162c-fab4-49d8-8f6f-1e9ed96ffaa7
source-git-commit: e7a53a4892a8769fc178f5f3f2b82201589177b2
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 1%

---

# Aperçu{#overview}

Adobe Experience Cloud Device Co-op est un programme qui permet aux participants de travailler ensemble pour mieux identifier les consommateurs à travers les points de contact numériques tout en assurant le niveau de confidentialité et de transparence le plus élevé. Device Co-op Experience Cloud permet aux marques participantes de reconnaître leurs clients afin de leur offrir des expériences plus personnalisées sur tous les appareils et applications, à grande échelle. Device Co-op est un service principal de Adobe Experience Cloud. Il est disponible pour les clients Adobe qui utilisent Analytics, Audience Manager, Media Optimizer ou Target.

## Avantages {#section-ba8d23e1e5174bea8f84aab4642d4809}

Device Co-op permet aux participants d’offrir à leurs clients une expérience de contenu meilleure et plus cohérente lorsqu’ils migrent entre les appareils. Pour ce faire, il établit des liens entre un groupe d’appareils utilisés par des consommateurs inconnus. Cette technologie permet aux marketeurs de comprendre et de répondre aux comportements des consommateurs sur tous les appareils. Les résultats fournissent des mesures d’engagement du site web plus précises, un contenu plus personnalisé et des expériences publicitaires plus ciblées sur la recherche, l’affichage et les réseaux sociaux. Participation à [!DNL Adobe Experience Cloud] Device Co-op aide nos membres à améliorer :

* **Compréhension du client :** Les rapports traditionnels peuvent révéler des informations pour un appareil spécifique. Mais les appareils et les canaux n&#39;achètent pas — les gens le font. Grâce à de meilleurs rapports, Device Co-op aide les analystes et les spécialistes du marketing à répondre aux vraies questions centrées sur les personnes que leur entreprise pose.
* **Personnalisation du contenu :** Les clients qui ne se connectent pas au site web ou à l’application d’une marque reçoivent généralement une expérience liée à l’appareil qu’ils utilisent à ce moment-là. Device Co-op aide les marketeurs à offrir des expériences cohérentes et précieuses basées sur les informations qu’une marque possède sur une personne, et pas seulement sur l’appareil qu’ils utilisent.
* **Efficacité des dépenses publicitaires :** Device Co-op contribue à réduire les budgets marketing en concentrant la publicité display sur les personnes, et non sur les appareils. Comme les limites de fréquence s’appliquent généralement à un seul appareil, une limite de 5 publicités par consommateur peut facilement se transformer en 5 publicités par appareil. Grâce à Device Co-op, les marketeurs peuvent optimiser leur retour sur investissement en ciblant la personne, et non l’appareil.
* **Reciblage sur plusieurs périphériques :** Atteignez vos clients grâce à la puissance du reciblage déverrouillé sur les mobiles, tablettes, navigateurs et autres appareils qu’ils utilisent tous les jours. La publicité est considérablement plus efficace si vous pouvez rester à l’esprit, et le reciblage entre appareils permet à votre marque de le faire exactement.

<!--
we may not want to share info in this with customers who have not signed. Also, removed directory from S3.
<p>Download our white-paper, <a href="https://marketing-stage.adobe.com/resources/help/en_US/mcdc/downloads/what_to_expect.pdf" format="https" scope="external"> What to Expect from the Device Co-op</a> for more information. </p>
-->

## Rôle de l’Adobe dans Device Co-op {#section-f23c1c442ceb4c44821f10ec9aa7b828}

Dans le [!DNL Device Co-op], [!DNL Adobe]:

* **est un gestionnaire de données :** Les membres de Device Co-op ne partagent pas directement les données entre eux. Au lieu de cela, [!DNL Adobe], agit en tant qu’intermédiaire pour que les données de lien d’appareil soient disponibles pour la coopérative au moyen de la fonction [!DNL Device Graph]. Les membres de Device Co-op peuvent utiliser ces données grâce à des fonctionnalités qui sont activées. [!DNL Experience Cloud] solutions.

* **Croit en l&#39;équité des données :** Le partage équitable des données est un concept important de Device Co-op. Tous [!DNL Device Co-op] les membres reçoivent une valeur relative à ce qu’ils contribuent. Si vous n’avez jamais interagi avec une personne anonyme au cours d’une visite de site ou d’une impression publicitaire, vous n’obtiendrez aucune information sur leurs appareils dans la variable [!DNL Device Graph]. Device Co-op aide les marques à reconnaître les consommateurs familiers à l’aide d’appareils inconnus.

* **Prend en charge les normes de confidentialité :** [!DNL Device Graph] Les données ne comprennent pas les informations d’identification personnelle (PII). L’exclusion des informations d’identification personnelles du graphique de périphérique permet [!DNL Adobe] respecter les normes de protection de la vie privée et maintenir la confiance des membres de la coopérative et des consommateurs.

## Fonctionnement {#section-7f7a0138e54349278fc463764f03cd4b}

Les membres de Co-op accorderont à l’Adobe un accès aux identifiants de connexion hachés cryptographiquement et aux données d’en-tête HTTP, qui masquent entièrement l’identité d’un consommateur. Adobe traite ces données pour créer des groupes d’appareils (&quot;grappes de périphériques&quot;) utilisés par une personne ou un foyer inconnu. Adobe fera ensuite apparaître ces groupes d’appareils par le biais de ses solutions de marketing numérique, de sorte que les membres de la Co-op puissent mesurer, segmenter, cibler et faire de la publicité directement pour les individus sur tous leurs appareils. Tout cela est possible sans révéler l’identité de l’utilisateur, car la variable [!DNL Device Co-op] *ne fait pas* partager des données personnelles telles que des noms, des adresses électroniques, des numéros de téléphone ou des données de visite de site, etc. ; parmi ses membres.

Ces règles permettent de répondre à d’importantes questions de confidentialité généralement associées aux technologies multi-appareils. En fait, avec la [!DNL Device Co-op], les consommateurs disposeront de contrôles de confidentialité qui dépasseront les normes de l’industrie. Le [!DNL Device Co-op] offre une transparence sans précédent en permettant aux consommateurs d’avoir des informations sur les marques participantes, ainsi que sur tous les appareils associés à l’appareil en cours d’utilisation. Voir [Device Graph : Processus internes et sortie](../processes/links.md#concept-e9526af3476b478aab7c57b9ed0bab7c) pour plus d’informations.

## Prise en main {#section-53a47ffdc5bf47c88cedcb92dd65444b}

Prenez quelques instants pour consulter la section [exigences d’appartenance](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43) si vous souhaitez participer ou en savoir plus sur l’événement [!DNL Device Co-op]. Voir aussi [Utilisation des données Device Co-op dans d’autres solutions Experience Cloud](../other-solutions/other-solutions.md#concept-46278a50cfca4e1ab83a3b35077a585f) pour un résumé de la façon dont les autres [!DNL Adobe] Les produits utilisaient ces données.
