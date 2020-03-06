---
description: Comment le graphique de périphériques analyse les données déterministes et probabilistes pour créer une carte qui relie les périphériques ensemble.
seo-description: Comment le graphique de périphériques analyse les données déterministes et probabilistes pour créer une carte qui relie les périphériques ensemble.
seo-title: Liens déterministes et probabilistes
title: Liens déterministes et probabilistes
uuid: 00693a0a-f73d-460d-84a4-b7c745b9fe0a
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031

---


# Deterministic and probabilistic links{#deterministic-and-probabilistic-links}

Comment le graphique de périphériques analyse les données déterministes et probabilistes pour créer une carte qui relie les périphériques ensemble.

Dans [!DNL Device Graph], les processus internes génèrent une hiérarchie des identités qui cartographie les périphériques et les associe à des individus anonymes. La sortie du graphique comprend des liens entre périphériques que vous pouvez utiliser pour le ciblage, ainsi que des données exposées dans certaines solutions Experience Cloud. The Adobe solutions that work with [!DNL Device Graph] data include Analytics, Audience Manager, Media Optimizer, and Target.

[!DNL Device Graph] analyse les données déterministes et probabilistes afin de dresser une carte reliant les différents périphériques. Les données déterministes relient les périphériques en fonction des informations d’ouverture de session hachées. Les données probabilistes relient les périphériques en fonction d’informations telles que les adresses IP et autres métadonnées. [!DNL Device Graph] associe les grappes de périphériques liés à une personne anonyme. Les marketeurs peuvent ainsi toucher des personnes plutôt que des périphériques. Dans [!DNL Device Graph], le propriétaire d’un périphérique constitue la représentation anonyme d’une personne réelle. Les liaisons déterministes et probabilistes contribuent à structurer l’identité de l’utilisateur.

>[!NOTE]
>
>Dans Adobe Experience Cloud Device Co-op, les termes tels que *périphérique*, *personne* et *identité* ont des significations spécifiques. For example, *device* can refer to physical hardware such as a phone or tablet and the applications that run on that hardware. Consultez le [glossaire](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c) pour en connaître les définitions.

## What are links? {#section-2df4c6f01eba49369993146df0661f13}

Il convient de ne pas oublier que nous parlons de liaisons dans le contexte du [!DNL Experience Cloud] Device Graph. Ici, il ne s’agit pas de connexions physiques entre des périphériques mais plutôt de la façon dont Device Graph associe différents périphériques à la même personne inconnue. Prenons l’exemple d’un téléphone mobile et d’un navigateur d’ordinateur. Ils peuvent être « liés » une fois que Device Graph a déterminé que ces deux périphériques sont utilisés par la même personne inconnue. Comme il est expliqué ci-après, Device Graph construit les identités à partir de liaisons déterministes et probabilistes. En outre, dans Device Graph, le propriétaire d’un périphérique constitue la représentation anonyme d’une personne réelle.

## Deterministic links {#section-33d41e828a674b398e36fe63da20ac09}

Les liaisons déterministes associent un périphérique à une personne en fonction d’un événement d’authentification (ex. : une ouverture de session sur un site à partir d’un périphérique). Cette action crée un identificateur anonyme, communément appelé un identifiant client. Voyons comment fonctionne la liaison déterministe. Dans cet exemple, la personne A ouvre une session sur un site d’actualités au moyen d’une application sur son périphérique mobile. Plus tard au cours de la même journée, cette personne A ouvre une nouvelle session sur ce site, mais cette fois via un navigateur sur son ordinateur portable.

![](assets/link1.png)

Selon les informations d’ouverture de session, Device Graph :

* sait que cette personne A s’est identifiée sur le site d’actualités depuis un téléphone mobile (via une application) mais aussi depuis un ordinateur portable (via un navigateur) ;
* relie ces périphériques à la personne A ;
* génère une identité en fonction des périphériques liés et associés à une personne anonyme.

![](assets/link2.png)

>[!NOTE]
>
>Neither the [!DNL Adobe Experience Cloud Device Co-op] or the [!DNL Device Graph] receives actual authentication information or personally identifiable information (PII) in this data. Members of the [!DNL Experience Cloud Device Co-op], pass in cryptographically hashed, unique consumer IDs to the Device Graph. L’identifiant client représente un utilisateur authentifié dans le graphique et protège sa vie privée.

## Probabilistic links {#section-5f5aa755da984f9d851f7cb380262998}

Les liaisons probabilistes s’appuient sur une solution algorithmique pour relier un périphérique à une personne, en fonction de caractéristiques et de métadonnées du type :

* Comportement de navigation
* Adresses IP
* Systèmes d’exploitation
* Identifiants publicitaires IDFA et GAID

Voyons comment fonctionne la liaison probabiliste. Dans cet exemple, la personne A navigue jusqu’à un site d’actualités sur sa tablette, puis plus tard sur son ordinateur. Toutefois, elle ne s’identifie pas sur ce site. Durant chacune de ces visites, la tablette et l’ordinateur partagent la même adresse IP.

![](assets/link3.png)

En fonction de ces informations, [!DNL Device Graph] évalue les schémas de partage d’adresses IP entre les deux périphériques et relie ces derniers si les résultats suggèrent qu’ils appartiennent à la personne A. Une hiérarchie des identités est ainsi établie selon des calculs de probabilité algorithmique.

![](assets/link4.png)

Dans cet exemple, Device Graph a pu relier les deux périphériques après qu’ils ont été utilisés pour accéder au même site d’actualités. Toutefois, les périphériques ne doivent pas forcément se connecter au même site pour être reliés. Imaginons, pour illustrer ce propos, que chaque périphérique de cet exemple accède à des sites web complètement différents. L’algorithme [!DNL Device Graph] peut encore créer une liaison probabiliste à l’aide des adresses IP partagées et de l’analyse d’autres données. Forte de ce processus, la liaison probabiliste s’avère un outil extrêmement performant pour les membres de [!DNL Experience Cloud] Device Co-op.

## Both types of data provide value {#section-43d22d8c10634edcb261e7bda6fdf323}

Les données déterministes et probabilistes sont complémentaires. Ainsi, s’il ne prend en compte que des données déterministes, un graphique Device Graph ne dresse qu’un portrait limité de l’identité de la personne. Sans authentification, un graphique Device Graph ne peut pas vous informer sur les autres périphériques et personnes qui consultent votre site. Les données probabilistes peuvent établir ces connexions et vous aider à toucher des périphériques, des personnes et des foyers non authentifiés.

Reste que les données déterministes n’en sont pas moins importantes. Elles peuvent par exemple améliorer la prise de décision probabiliste en supprimant les faux liens générés dans les lieux où les signaux probabilistes abondent et se chevauchent (cafés, bibliothèques, aéroports, etc.).

Grâce à la combinaison de ces deux types de données, Device Graph vous dresse un portrait plus complet de l’identité d’une personne qu’avec un seul de ces types de données.

![](assets/link5.png)

