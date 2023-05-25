---
description: Présentation du cluster BigBlueButton de l'ESR
---

# Infrastructure BigBlueButton de l'ESR

L'infrastructure BigBlueButton de l'ESR est opérée par [France Université Numérique](https://www.france-universite-numerique.fr/), hébergée par [Scaleway](https://www.scaleway.com) et infogérée par [Arawa](https://www.arawa.fr/).

Elle se compose de :

- Serveurs BigBlueButton autoscalés en nombre variable en fonction de la demande et sur lesquels ont lieu les classes virtuelles,
- Un load balancer Scalelite qui gère l'authentification multi-tenant des connections en provenance des universités et répartit les classes virtuelles entre les différents serveurs BigBlueButton en fonction de leur charge respective,
- Un espace de stockage objet pour la persistence des documents liés aux classes virtuelles : enregistrements video, notes partagées, présentations, etc.
- Un serveur Turn pour permettre l'accès aux classes virtuelles aux participants pour lesquels le traffic UDP est bloqué.

![Architecture BigBlueButton](/assets/bigbluebutton_esr_archi.png)
