---
description: Device Graph analyse les données déterministes et probabilistes afin de créer une carte qui relie les périphériques.
seo-description: How the Device Graph analyzes deterministic and probabilistic data to build a map that links devices together.
seo-title: Deterministic and probabilistic links
title: Liens déterministes et probabilistes
uuid: 00693a0a-f73d-460d-84a4-b7c745b9fe0a
exl-id: e9bd2b7a-7d39-425d-adbb-298944009fcc
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Liens déterministes et probabilistes{#deterministic-and-probabilistic-links}

Device Graph analyse les données déterministes et probabilistes afin de créer une carte qui relie les périphériques.

Dans le [!DNL Device Graph], les processus internes créent une hiérarchie d’identités qui mappe les périphériques et les connecte à des personnes individuelles anonymes. La sortie du graphique comprend des liens multi-appareils que vous pouvez utiliser pour le ciblage, ainsi que des données exposées dans des solutions Experience Cloud sélectionnées. Les solutions d’Adobe qui fonctionnent avec [!DNL Device Graph] Les données comprennent Analytics, Audience Manager, Media Optimizer et Target.

Le [!DNL Device Graph] analyse les données déterministes et probabilistes afin de créer une carte qui relie les périphériques. Les données déterministes relient les appareils en fonction des informations de connexion hachées. Les données probabilistes relient les périphériques en fonction d’informations telles que des adresses IP et d’autres métadonnées. Le [!DNL Device Graph] associe les grappes d’appareils liées à une personne anonyme. Ces connexions permettent aux spécialistes du marketing numérique d’atteindre des personnes plutôt que des appareils. Dans le [!DNL Device Graph], le propriétaire d’un appareil est la représentation anonyme d’une personne réelle. Les liens déterministes et probabilistes permettent de construire une structure d&#39;identité de l&#39;utilisateur.

>[!NOTE]
>
>Dans Adobe Experience Cloud Device Co-op, les termes tels que *appareil*, *personne*, et *identité* ont des significations spécifiques. Par exemple : *appareil* peut faire référence au matériel physique, tel qu’un téléphone ou une tablette, ainsi qu’aux applications qui s’exécutent sur ce matériel. Voir [glossaire](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c) pour les définitions.

## Que sont les liens ? {#section-2df4c6f01eba49369993146df0661f13}

Quand nous parlons de liens, il est important de garder à l&#39;esprit ce qu&#39;ils sont réellement dans le contexte de la [!DNL Experience Cloud] Device Graph. Dans ce contexte, les liens ne sont pas des connexions physiques entre appareils. À la place, un lien est la manière dont Device Graph associe différents appareils à une même personne inconnue. Par exemple, supposons que nous ayons un téléphone mobile et un navigateur de bureau. Le téléphone et le navigateur peuvent être considérés comme &quot;liés&quot; une fois que Device Graph a déterminé que ces deux appareils sont utilisés par la même personne inconnue. Comme vous le verrez ci-dessous, Device Graph crée des identités avec des liens déterministes et probabilistes. Et, dans Device Graph, le propriétaire d’un appareil est la représentation anonyme d’une personne réelle.

## Liens déterministes {#section-33d41e828a674b398e36fe63da20ac09}

Les liens déterministes associent un appareil à une personne en fonction d’un événement d’authentification (par exemple, une action de connexion à un site à partir d’un appareil). Cette action crée un identifiant anonyme, connu sous le nom d’identifiant de consommateur. Regardons comment fonctionne la liaison déterministe. Dans cet exemple, la personne A se connecte à un site de nouvelles par le biais d’une application sur son appareil mobile. Plus tard dans la journée, la personne A se reconnecte, mais cette fois-ci par le biais d’un navigateur sur son ordinateur portable.

![](assets/link1.png)

En fonction des informations de connexion, Device Graph :

* Sait que la Personne A s’est authentifiée sur le site d’actualités avec une combinaison de téléphone/application mobile et d’appareil portable/navigateur.
* Associe ces périphériques à la personne A.
* Construit une identité basée sur des appareils liés associés à une personne anonyme.

![](assets/link2.png)

>[!NOTE]
>
>Ni les [!DNL Adobe Experience Cloud Device Co-op] ou le [!DNL Device Graph] reçoit des informations d’authentification réelles ou des informations d’identification personnelle (PII) dans ces données. Les membres de [!DNL Experience Cloud Device Co-op], transmettez des identifiants consommateurs uniques hachés cryptographiquement à Device Graph. L’ID de consommateur représente un utilisateur authentifié dans le graphique et protège la vie privée des clients.

## Liens probabilistes {#section-5f5aa755da984f9d851f7cb380262998}

Les liens probabilistes connectent algorithmiquement un appareil à une personne, en fonction de caractéristiques et de métadonnées telles que :

* Comportement de navigation
* Adresses IP
* Systèmes d’exploitation
* Identifiants IDFA et GAID

Regardons comment fonctionne la liaison probabiliste. Dans cet exemple, la personne A accède à un site d’actualités sur sa tablette, puis plus tard sur un ordinateur de bureau. Lors de la navigation, la personne A ne se connecte pas au site d’actualités. Au cours de chaque visite distincte, la tablette et le bureau partagent la même adresse IP.

![](assets/link3.png)

Sur la base de ces informations, la variable [!DNL Device Graph] évalue les schémas de partage d’adresses IP entre les deux appareils et relie ces derniers si les résultats suggèrent qu’ils appartiennent à la personne A. Le résultat final est une hiérarchie d’identité dérivée des calculs de probabilité algorithmique.

![](assets/link4.png)

Dans cet exemple, Device Graph a lié les deux appareils une fois qu’ils ont été utilisés pour accéder au même site d’actualités. Mais il n’est pas nécessaire de voir les périphériques sur le même site pour qu’ils soient liés. Pour illustrer ce point, supposons que chaque périphérique de cet exemple visite des sites web complètement différents. Le [!DNL Device Graph] L’algorithme peut toujours créer une liaison probabiliste à partir de son adresse IP partagée et d’une analyse d’autres données. Ce processus contribue à rendre la liaison probabiliste si puissante pour les membres de l&#39;équipe [!DNL Experience Cloud] Device Co-op.

## Les deux types de données apportent de la valeur {#section-43d22d8c10634edcb261e7bda6fdf323}

Les données déterministes et probabilistes se complètent. En revanche, un graphique d’appareil qui inclut uniquement des données déterministes vous donne une vue limitée de l’identité d’une personne. Sans authentification, un graphique d’appareil ne peut pas vous informer sur d’autres appareils et personnes qui parcourent votre site. Les données probabilistes peuvent établir ces connexions et vous aider à atteindre des appareils, des personnes et des ménages non authentifiés.

Cependant, les données déterministes sont importantes également. Elle peut, par exemple, améliorer la prise de décision probabiliste en supprimant les faux liens générés dans les endroits où les signaux probabilistes sont abondants et se chevauchent (cafés, bibliothèques, aéroports, etc.).

Avec les deux types de données, Device Graph vous donne une vue plus complète de l’identité d’une personne que de l’un ou l’autre de ces types de données.

![](assets/link5.png)
