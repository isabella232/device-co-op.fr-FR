---
description: A propos du partage de liens dans le graphique de périphériques.
seo-description: A propos du partage de liens dans le graphique de périphériques.
seo-title: Partage de liens dans le graphique de périphériques
title: Partage de liens dans le graphique de périphériques
uuid: 6c7202f0-c6d9-48a4-82ad-ee57d7a518a0
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031

---


# Link sharing in the Device Graph{#link-sharing-in-the-device-graph}

A propos du partage de liens dans le graphique de périphériques.

The [!DNL Device Graph] shares deterministic and probabilistic links with different members of the Adobe Experience Cloud Device Co-op. Link sharing is what makes the [!DNL Device Co-op] so powerful. Il complète vos connaissances des périphériques associés à une personne anonyme, à condition d’avoir déjà été en contact avec l’un de ses périphériques.

## Device Graph summary review {#section-7858e9f61b5644c981ffb53626fcc19d}

Avant de commencer, prenons quelques instants pour revoir le fonctionnement de [!DNL Device Graph]. Members of the [!DNL Device Co-op] send data to the [!DNL Device Graph]. L&#39; [!DNL Device Graph] utilisateur utilise ces données pour construire l&#39;identité d&#39;une personne à partir de liens [](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931) déterministes et probabilistes entre des dispositifs. En tant que participant à [!DNL Device Co-op], ces liens vous fournissent des informations sur la relation entre vos utilisateurs authentifiés, les autres utilisateurs et leurs périphériques. Examinons son fonctionnement dans la section ci-dessous.

## Link sharing example {#section-cb410d827cf14f76bc9b0bd4d31ed767}

L’exemple suivant illustre l’efficacité du partage des liaisons dans Device Co-op. Dans cet exemple, deux sociétés fictives sont impliquées : la société Média et la société Finance. Both companies are members of the [!DNL Device Co-op]. La personne A est un consommateur qui ouvre une session sur les sites web de chaque société, ou les consulte, depuis plusieurs périphériques.

![](assets/share1.png)

Puisque la personne A s’est authentifiée sur le site d’actualités de Média depuis son téléphone mobile et sa tablette, cette dernière lui a attribué un identifiant client (ID) qu’elle transmet à [!DNL Device Graph] sous la forme d’un hachage cryptographique. La société Finance connaît déjà ces périphériques, mais la personne A n’a jamais ouvert de session sur son site. Par conséquent, Finance ne sait pas si ces périphériques sont liés, ni comment ils le sont entre eux ou avec la personne A.

![](assets/share2.png)

En fonction du hachage cryptographique de l’identifiant client, [!DNL Device Graph] reconnaît que ces périphériques sont liés entre eux et à une personne donnée. Pour les entreprises qui ne participent pas au programme [!DNL Device Co-op], les visites sur ces sites sont répertoriées comme des visites depuis des périphériques distincts et aléatoires. Ainsi, une fois que [!DNL Device Graph] a récupéré l’identifiant haché :

* il sait que le téléphone mobile et l’ordinateur portable sont liés ;
* il en déduit que la société Finance veut aussi savoir si le téléphone mobile et l’ordinateur portable sont liés.

Bilan, [!DNL Device Graph] partage maintenant la liaison qui relie ces périphériques pour Média avec Finance. Durant ce processus, [!DNL Device Graph] duplique et partage la liaison pour les membres de la coopérative.

![](assets/share3.png)

At this point, the [!DNL Device Graph] performed its role successfully. Les société Média et Finance ont clairement défini une identité. Elles peuvent toucher précisément la personne A sur tous ses périphériques.

## Privacy and link sharing {#section-7b566018b3304420a4b3e4c079826110}

Pour les membres de [!DNL Device Co-op], il est crucial de préserver la vie privée des consommateurs et l’intégrité des données tout au long du processus de partage de liaisons. Au cours de ce processus de partage de liaisons et d’identification des consommateurs, [!DNL Device Graph] n’a pas :

* informé la société Finance que la liaison provenait de la société Média ;
* partagé l’identifiant client utilisé par un membre de [!DNL Device Co-op] avec un autre ;
* fourni d’autres informations que la liaison entre le périphérique mobile et l’ordinateur portable.

## Étapes suivantes {#section-ac6e61f1eb6e45b1bb4be8ece39147c7}

La lecture de la documentation sur l’identité, la liaison et le partage de liaisons devrait vous permettre de bien comprendre comment [!DNL Device Graph] réconcilie les données en interne. À l&#39;étape suivante, nous vous recommandons d&#39;examiner notre documentation qui décrit comment le concept d&#39;un *`known device`* produit des liens inter-périphériques vers les membres Device Co-op. Voir Périphériques [](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) connus et Périphériques [](../processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40)inconnus.
