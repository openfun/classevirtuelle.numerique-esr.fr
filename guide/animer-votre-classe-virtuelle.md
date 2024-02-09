---
description: >-
  Cette rubrique vise à vous aider à prendre en main les principales
  fonctionnalités de BigBlueButton
---

# 4. Animer la classe virtuelle avec BigBlueButton

En cliquant sur le bouton `Rejoindre` à l'heure prévue, un nouvel onglet s'ouvre et vous êtes désormais dans la salle BigBlueButton. Vous pouvez alors profiter de toutes les fonctionnalités de la version 2.6 de cette solution.

![Ecran de lancement par défaut de la solution BBB pour l'ESR](/assets/animer-v2.5.png)

{% hint style="success" %}
Vous trouverez ci-dessous un aperçu des principales fonctionnalités pour bien démarrer avec BBB. Ce logiciel libre propose néanmoins un très large panel d'options : si vous n'avez pas trouvé réponse à vos questions ici, vous pouvez consulter les ressources listées dans la partie [Pour aller plus loin](/guide/animer-votre-classe-virtuelle.md#pour-aller-plus-loin).
{% endhint %}

## Activation du micro et de la caméra

### Rejoindre l'audio de la réunion

Une fois dans la salle, tous les utilisateurs devront choisir entre `Microphone` et `Ecoute seule`

![Choix d'activer le micro et de rejoindre la classe en écoute seule](/assets/audio-micro.png)

et valider un test d'écho.

![Cliquer sur Oui permet de rejoindre la salle](/assets/audio-echo.png)

En cas de problème, la réponse `Non` proposera des choix de microphone et haut-parleur supplémentaires :

![](/assets/audio-modifier-parametres.png)

Le mode **Ecoute seule** ne permet pas de prendre la parole. Il est néanmoins possible de changer d'avis et de rejoindre la discussion en cliquant sur `Quitter l'audio de la réunion` (icône **Casque**) et en modifiant son choix.

![Animation qui montre comment quitter et rejoindre l'audio de la réunion](/assets/marsha-bbb-audio-change.gif)

{% hint style="success" %}
Vous pouvez recommander cette manipulation aux étudiants entrés dans la salle en écoute seule mais qui souhaitent finalement prendre la parole.
{% endhint %}

### Partager sa caméra

La caméra des participants n'est pas activée par défaut.

Il faut cliquer sur la bouton `Partager webcam` <img src="/assets/animer-partager-webcam.png" alt="" data-size="line"> pour l'activer et en autoriser l'utilisation via votre navigateur web : <img src="/assets/animer-webcam-navigateur.png" alt="" data-size="line">

Un menu vous propose alors de choisir **votre caméra**, sa **qualité de diffusion** et **un arrière-plan** :

![](/assets/animer-webcam.png)

{% hint style="info" %}
En tant que modérateur, vous avez la possibilité d'épingler <img src="/assets/animer-cam-pin.png" alt="" data-size="line"> ou désépingler votre caméra et celle des autres participants <img src="/assets/animer-cam-unpin.png" alt="" data-size="line">
{% endhint %}

## Accueil des participants

### Gestion de la salle d'attente

Par défaut, l'entrée des participants (non modérateurs) se fera dans une salle d'attente : <img src="/assets/animer-salle_dattente.png" alt="" data-size="line">

Vous serez notifié-e de leur arrivée : <img src="/assets/animer-salle_dattente-arrivee.png" alt="" data-size="line">

En cliquant sur `Utilisateurs en attente`, vous pourrez alors :

* autoriser ou rejeter les demandes **de façon globale** (en cliquant sur `Autoriser tout utilisateur authentifié` ou `Autoriser tout le monde`)
* **mémoriser ce choix** pour tout nouvel arrivant en cochant la case `Se rappeler du choix`
* traiter le demandes **au cas par cas** avec la liste des utilisateurs en attente
* écrire un message à tous les utilisateurs en attente ou à des personnes précises

![](/assets/animer-gerer-attente.png)

{% hint style="success" %}
Vous pouvez désactiver la salle d'attente depuis les options de configuration de la salle : [Outils et applications](/guide/configurer-votre-classe-virtuelle.md#outils-et-applications)
{% endhint %}

### Discussion publique et messages privés

Si vous avez saisi un `Texte de bienvenue` à l'étape de configuration, il s'affichera dans le chat.

Vous pouvez désormais participer à la **discussion publique** ou bien envoyer un **message privé** à un participant en cliquant sur son nom d'utilisateur.

![Exemple animé d'utilisation du chat dans BBB](/assets/bbb-discussions.gif)

## Modération et présentation

### Les rôles de modérateur et participant normal

Si vous êtes membre de l'équipe pédagogique du cours, vous aurez automatiquement un statut de modérateur dans BigBlueButton. Les apprenants entreront en tant que simples participants.

Dans BBB, cette différence est marquée visuellement (**carré** pour les modérateurs, **rond** pour les participants) et il est possible de modifier le statut de chaque participant :

![Promouvoir un participant comme modérateur](/assets/moderation-statut.png)

![Rétrograder un modérateur en simple participant](/assets/moderation-statut-back.png)

En tant que modérateur, vous avez les permissions suivantes :&#x20;

![Permissions du rôle modérateur pour chaque participant](/assets/moderation-statut-permissions.png)

Une gestion globale des utilisateurs est également réservée au modérateurs (via la roue crantée) :&#x20;

![Permissions du rôle modérateur pour tous les participants](/assets/moderation-statut-options-config.png)

{% hint style="info" %}
Pour plus de précisions sur les différentes permissions accessibles aux modérateurs, vous pouvez consulter la vidéo [Découvrir l'interface vue modérateur (PodEduc)](https://podeduc.apps.education.fr/video/3370-decouvrir-linterface-vue-moderateur/).
{% endhint %}

### Le rôle de présentateur

Dans BigBlueButton, il ne peut y avoir qu'**un seul présentateur à la fois**.

Ce rôle peut être donné à d'autres participants en cliquant sur leur nom d'utilisateur (sans pour autant devoir les promouvoir comme modérateurs).

![Donner le rôle de présentateur à un participant normal](/assets/presentation01.png)

Si vous êtes modérateur, vous pouvez "reprendre la main" en cliquant sur votre nom d'utilisateur puis `Devenir présentateur`.

![Reprendre le rôle de présentateur à un participant](/assets/presentation02.png)

Vous pouvez également cliquer sur le bouton d'`Actions` (cercle bleu dans le coin inférieur gauche) derrière lequel se trouvent les options de présentation.

![Donner le rôle de présentateur en cliquant sur les options de présentation](/assets/presentation03.png)

**Seul le rôle de présentateur peut :**

* Gérer les documents de présentation
* Lancer un sondage
* Partager une vidéo externe
* Sélectionner un utilisateur aléatoirement
* Partager son écran
* Faire défiler les diapositives
* Ecrire ou dessiner sur le tableau blanc (sauf activation de la fonctionnalité pour toutes les personnes présentes)

{% hint style="info" %}
Pour plus de précisions sur les différentes permissions accessibles au présentateur, vous pouvez consulter la vidéo [Les outils du présentateur (PodEduc)](https://podeduc.apps.education.fr/video/3496-les-outils-du-presentateur/).
{% endhint %}

## Enregistrement de la classe

Les classes virtuelles BBB peuvent être enregistrées. Pour cela, en tant que modérateur, cliquez sur le bouton `Commencer l'enregistrement` en haut de la salle et validez le message en sélectionnant `Oui`.

![Lancer l'enregistrement de la classe virtuelle](/assets/marsha-bbb-record-yes.gif)

Vous pouvez arrêter et reprendre l'enregistrement autant de fois que nécessaire.

![Mettre en pause et reprendre l'enregistrement](/assets/marsha-bbb-record-stop.gif)


{% hint style="info" %}
Tous les moments enregistrés au cours d'une session sont proposés dans un seul fichier au format .mp4 (voir [#enregistrements](configurer-votre-classe-virtuelle.md#enregistrements "mention")).
{% endhint %}

## Sondages et "diapositives intelligentes"

### Lancer un sondage

Vous pouvez initier des sondages auprès de vos étudiants durant votre classe virtuelle.

Pour lancer un sondage, vous devez avoir [le rôle de présentateur](/guide/animer-votre-classe-virtuelle.md#le-rôle-de-présentateur), cliquer sur le bouton d'`Actions` en bas à gauche de la présentation et choisir `Lancer un sondage` dans le menu.

![Appuyer sur le bouton d'Actions en tant que présentateur](/assets/bbb-ajout-sondage.png)

Vous avez plusieurs types de réponses prédéfinies sous forme de **Question à choix unique** ou d'un **champ de réponse libre** (`Réponse utilisateur`) :

![Types de réponses prédéfinies](/assets/bbb-sondages-predefinis.png)

Depuis cette interface, vous pouvez autoriser les étudiants à donner plusieurs réponses en cochant la case `Question à choix multiple` ainsi que déterminer si les réponses seront anonymes ou pas au niveau du sélecteur `Sondage Anonyme`.

![](/assets/bbb-sondage-qcm_anon.png)

Vous pouvez ajouter autant de choix que nécessaire directement depuis les champs de réponse depuis le champ `Renseigner les valeurs du sondage` (copier-coller ou glisser-déposer d'un fichier au format .txt)

![Exemple animé pour ajouter des choix à partir d'un fichier .txt](/assets/bbb-sondage-txt.gif)

Pour lancer le sondage, cliquez sur le bouton `Débuter un sondage` et laissez un temps à vos étudiants pour répondre avant de cliquer sur `Publier le sondage`. Cela aura pour effet d'afficher les résultats dans le coin inférieur droit de la présentation.&#x20;

![Exemple animé de diffusion d'un sondage (vue présentateur à gauche et participant normal à droite)](/assets/bbb-sondage-reponse.gif)

### Préparer vos sondages avec les "diapositives intelligentes"

Les diapositives intelligentes vous permettent de préparer un sondage en amont de la classe en incluant vos questions dans la présentation. BigBlueButton détecte quand une question est posée et offre une option de sondage rapide au présentateur, sans avoir besoin d'initier le sondage depuis le menu d'`Actions`.

Pour créer des diapositives intelligentes, il faut s'assurer d'utiliser le format : "question ?" suivie des "options de réponse". Il est recommandé d'utiliser les options de réponse suivantes pour de meilleurs résultats :

* Vrai / Faux
* Oui / Non
* Choix multiples

Si vous avez préparé votre présentation avec une question et des choix de réponse, un bouton de lancement rapide apparaîtra dans le coin inférieur gauche de la présentation.

![](/assets/bbb-smart-slides-detail.png)

A noter que vous pouvez préparer plusieurs questions sur une même page. Dans ce cas, nous vous recommandons de vérifier en amont que BBB détecte bien toutes vos questions.

![Exemple animé de lancement d'un sondage rapide avec plusieurs questions](/assets/bbb-smart-slides.multiple.gif)

{% hint style="info" %}
Le site PodEduc propose un tutoriel pour la mise en place des sondages automatiques sur BBB : [Créer un sondage automatique à partir d'un PDF](https://podeduc.apps.education.fr/video/5530-creer-un-sondage-automatique-a-partir-dun-pdf/)

Vous pouvez aussi vous référer à [cet article du centre d'aide BigBlueButton](https://support.bigbluebutton.org/hc/en-us/articles/1500005216661-) (en anglais).
{% endhint %}

## Outils de collaboration

### Notes partagées

Si vous avez activé les notes partagées, vos étudiants et vous-même pouvez collaborer sur un même document de traitement de texte.

![Exemple animé d'utilisation des notes partagés (rôle de modérateur à gauche, participant à droite)](/assets/bbb-notes-partagees.gif)

Chaque participant peut télécharger les notes partagées à tout moment en cliquant sur l'icône de droite :

![](/assets/bbb-telecharger-notes.png)

Vous pouvez verrouiller l'édition des notes partagées pour les participants. Seuls les modérateurs pourront alors les éditer.

![Exemple animé de verrouillage des notes partagées](/assets/bbb-notes-verrouillees.gif)

{% hint style="success" %}
En cliquant sur le pseudonyme d'un participant et en cliquant sur `Débloquer` <img src="/assets/bbb-notes-debloquer.png" alt="" data-size="line"> vous lui permettez de contribuer aux notes partagées sans pour autant débloquer les autres participants.
{% endhint %}

### Tableau blanc collaboratif

**En tant que présentateur**, vous pouvez utiliser une palette d'outils pour enrichir votre présentation en temps réel. Par défaut, l'icône **Main** est sélectionnée, ce qui affiche un pointeur sur votre présentation pour indiquer les points saillants.

#### Éléments graphiques

La première ligne d'outils vous permet de choisir l'élément graphique à afficher sur votre présentation : pointeur (**main**), **texte**, élément géométrique (**ligne**, **ellipse**, **triangle**, **rectangle**) ou dessin (**crayon**).

![Exemple animé pour sélectionner un outil graphique](/assets/bbb-tableau-outils.gif)

#### Taille et couleurs

Les 2e et 3e lignes d'outils permettent de modifier la taille et la couleur du texte ou de l'élément graphique sélectionné :

![Exemple animé pour modifier la taille et la couleur des éléments](/assets/bbb-taille-couleur.gif)

#### Annuler et effacer les annotations

La flèche circulaire <img src="/assets/bbb-annuler-annot.png" alt="" data-size="line">vous permet d'annuler le dernier élément ajouté tandis que la corbeille<img src="/assets/bbb-effacer-annot.png" alt="" data-size="line"> supprime toutes les annotations ajoutées à votre présentation.

![Exemple animé d'annulation et de suppression des annotations](/assets/bbb-tableau-annuler.gif)

A noter qu'il est possible d'utiliser le tableau blanc sur mobile en cliquant sur l'icône suivante <img src="/assets/bbb-tableau-mobile.png" alt="" data-size="line">. Cela activera les contacts de la paume de la main sur écran tactile.

#### Rendre le tableau blanc collaboratif (mode multi-utilisateurs)

Pour permettre à vos étudiants de collaborer sur votre support de présentation ou une diapositive blanche, vous pouvez cliquer sur l'icône `Activer le mode multi-utilisateurs`.

Tous les participants pourront alors écrire et dessiner sur la présentation.

Pour désactiver la collaboration sur le tableau (et retirer éventuellement les annotations), il suffit de recliquer sur l'option.

![Exemple animé d'utilisation du mode multi-utilisateurs](/assets/bbb-tableau-multi.gif)

{% hint style="info" %}
A noter qu'à partir de la version 2.6, le tableau blanc collaboratif de BigBlueButton est remplacé par l'outil **tl;draw** que vous pouvez tester dès à présent à cette adresse [https://www.tldraw.com/](https://www.tldraw.com/)
{% endhint %}

### Réunion privées

Sur BigBlueButton il est possible de répartir vos étudiants en sous-groupes dans des salles annexes (ou "breakout rooms").&#x20;

Pour ce faire, cliquez sur la roue crantée au-dessus de la liste des utilisateurs et sélectionnez `Créer des réunions privées`.

![](/assets/bbb-breakoutrooms01.png)

Une série d'options vous est proposée sur la page qui s'ouvre :&#x20;

* `Nombre de réunions` pour choisir le nombre de salles à créer
* `Durée (minutes)` (ce qui créera un compte à rebours visible par tous)
* `Autoriser les participants à choisir la salle de réunion privées qu'ils souhaitent rejoindre` (à cocher pour leur permettre de choisir leur salle)
* `Affecter aléatoirement` ou `Réinitialiser les affectations`
* Vous pouvez également glisser-déposer manuellement les utilisateurs dans chacune des salles créées.

![Interface de création des réunions privées](/assets/bbb-breakoutrooms02.png)

Côté participant, un nouvel onglet s'ouvrira pour accepter de rejoindre la réunion privée en cliquant sur le bouton `Rejoindre la réunion` :

![](/assets/bbb-breakoutrooms03.png)

Pour fermer les salles annexes avant la fin du temps imparti, vous pouvez ouvrir le volet `Salle de réunion privée` et sélectionner `Clôturer les réunions privées`.

![](/assets/bbb-breakoutrooms04.png)

{% hint style="info" %}
Pour plus d'informations, le site PodEduc propose un tutoriel pour la mise en place des réunions privées sur BBB : [Gérer les réunions privées (ateliers)](https://podeduc.apps.education.fr/video/3687-gerer-les-reunions-privees-ateliers/)
{% endhint %}

## Tableau de bord d'activité des participants

Pour un suivi précis des événements qui se sont produits durant la classe virtuelle (présence, chronologie, participation au chat, sondages et activités), les modérateurs peuvent accéder, via la roue crantée du panneau de gauche, à un `Tableau de bord d'activité des participants`.

![Accéder au tableau de bord d'activité des participants](/assets/dashboard01.png)

Celui-ci s'ouvrira dans un nouvel onglet.

![Vue d'ensemble du tableau de bord d'activité des participants](/assets/dashboard02.png)

Les données peuvent être consultées de façon interactive.

![Chaque onglet permet d'accéder à des statistiques spécifiques](/assets/dashboard03-marsha-bbb-stats.gif)

Elles peuvent aussi être téléchargées au format .csv en cliquant sur `Télécharger les données de la session` (dans le coin inférieur droit du tableau) :\

![](/assets/dashboard04.png)

{% hint style="danger" %}
Attention : **fermer la classe virtuelle réinitialise toutes les données**. Assurez-vous de récupérer ce qui vous est utile : discussion publique, notes partagées, données de la session ou annotations sur le tableau blanc collaboratif. &#x20;
{% endhint %}

## Pour aller plus loin

Nous proposons dans ce guide un bref tour d'horizon des principales fonctionnalités de BBB mais vous pouvez également vous référer à [la documentation officielle](https://bigbluebutton.org/teachers/tutorials/) (en anglais) qui comporte [des vidéos](https://www.youtube.com/playlist?list=PLeSl48Y1rgh9Cta0kM7IjjHarLRFeXlCF) et [des articles](https://support.bigbluebutton.org/hc/en-us/categories/1500000517381-BigBlueButton-HTML5) dédiés à la prise en main de l'outil.

De nombreux tutoriels ont aussi été réalisés en français, parmi lesquels :

* [les vidéos du portail PodEduc](https://podeduc.apps.education.fr/videos/?tag=bbb) de l'Education nationale (plusieurs fois citées dans ce guide)
* [le guide PDF](https://documentation.unistra.fr/Catalogue/Outils_collaboratifs/BigBlueButton/guide_bigbluebutton.pdf) par la Direction du numérique de l'Université de Strasbourg (à partir de la page 13).
* [le guide du Centre d'aide et de support au numérique](https://support.unilim.fr/multimedia-et-visioconference/visio-et-web-conference/bigbluebutton/) de l'Université de Limoges.

Les parties que vous seront utiles sont uniquement celles dédiées au logiciel BBB en lui-même car les solutions proposées dans le cadre du Plan de relance sont documentés ici-même.

{% hint style="success" %}
La version qui vous proposée dans le cadre du Plan de relance suivra les mises à jour de BigBlueButton. [Consultez cet article](https://docs.bigbluebutton.org/new-features) (en anglais) pour vous informer sur les nouveautés attendues avec la version 2.6 !
{% endhint %}

Retrouvez dans la rubrique suivante des recommandations pour terminer votre classe virtuelle.