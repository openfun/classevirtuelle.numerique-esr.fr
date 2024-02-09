---
description: >-
  Intégrez une classe virtuelle dans Moodle (versions 3.x ou 4.x) selon la
  modalité choisie par votre DSI.
---

# Depuis le Moodle de votre établissement

## Prérequis

Vous pouvez accéder à la solution de classes virtuelles via l’une des modalités suivantes, selon les mécanismes mis en place dans le Moodle de votre établissement par votre DSI.

* **En utilisant le plugin BBB pour Moodle** : vos étudiants voient directement dans l’espace de cours Moodle le lien vers la classe virtuelle et peuvent la rejoindre d’un simple clic. Seuls les étudiants inscrits au cours peuvent accéder à la classe virtuelle.
* **En utilisant l'activité de classes virtuelles disponible dans le cours Moodle via le standard LTI[^1]**, vous pourrez bénéficier de fonctionnalités de planification, d'invitation, d'enregistrement, d'import de documents et de paramétrage en amont. Toutes ces fonctionnalités sont documentées à l'étape suivante [configurer-votre-classe-virtuelle.md](../configurer-votre-classe-virtuelle.md "mention").

{% hint style="info" %}
Pour installer le passeport LTI ou le plugin BBB permettant l'accès à la solution dans Moodle, votre DSI peut contacter l'équipe technique de FUN en utilisant [ce formulaire de demande](https://www.fun-mooc.help/hc/fr/requests/new?ticket_form_id=9122250595357).
{% endhint %}

:bulb: **Consultez votre DSI pour savoir quelle modalité a été choisie au moment de l'installation.**

## Créer votre ressource classe virtuelle dans un cours

### Ajouter une ressource

A l'endroit où vous souhaiter ajouter votre classe, basculez en `Mode d'édition`.

![Activer le mode d'édition](/assets/moodle4-edition-button.gif)

Dans la section du cours de votre choix, choisissez `Ajouter une activité ou une ressource`.

![Ajouter une ressource](/assets/moodle4-ajouter_ressource.png)

Choisissez l'activité de classe virtuelle installée par votre DSI (plusieurs visuels possibles).

{% hint style="warning" %}
L'affichage du nom et de l'icône peuvent varier en fonction de la customisation choisie par votre DSI.

De même, la solution BBB peut se trouver au niveau du sélecteur d'activités ou être accessible via l'activité `Outil externe`.
{% endhint %}

{% tabs %}
{% tab title="Installation LTI" %}
![Sélecteur d'activité avec icône par défaut (Moodle 4.1)](/assets/moodle4-activite_cv.png)
{% endtab %}

{% tab title="Plugin BigBlueButton" %}
![Sélecteur d'activité avec icône par défaut (Moodle 4.1)](/assets/moodle4.activite_plugin_bbb.png)
{% endtab %}
{% endtabs %}

### Ajouter et paramétrer une nouvelle classe BigBlueButton

{% hint style="danger" %}
A partir de cette étape, les fonctionnalités et l'affichage varieront significativement selon le type d'installation choisie par votre DSI : **installation LTI** ou **plugin BigBlueButton**.
{% endhint %}

Choisissez le cas d'usage qui correspond à votre installation :

{% tabs %}
{% tab title="Installation LTI" %}
Sur la page **Ajout Outil externe**, cliquez sur `Sélectionner un contenu`.

![](/assets/moodle4-lti-ajout_contenu.png)

Dans la fenêtre qui s'ouvre, cliquez sur `Ajouter une classe virtuelle` (ou réutilisez une classe virtuelle déjà créée).

![](/assets/moodle4-lti-nouvelle_cv.png)

La fenêtre se ferme et il vous suffit de cliquer sur le bouton `Enregistrer et afficher` pour accéder à la classe virtuelle :

![](/assets/moodle4-enregistrer_afficher.png)

![Affichage de la classe virtuelle en LTI dans Moodle 4.1](/assets/moodle4-nouvelle_classe.png)

Toutes ces étapes sont résumées dans cette animation :

![Cet exemple animé indique comment ajouter une classe virtuelle sur Moodle 4.1](/assets/Classe-virtuelle-add.gif)

Rendez-vous à l'étape suivante pour [Configurer votre classe virtuelle](../configurer-votre-classe-virtuelle.md) !
{% endtab %}

{% tab title="Plugin BigBlueButton" %}
{% hint style="info" %}
Les fonctionnalités présentées ci-après correspondent au plugin BigBlueButton préconfiguré sur les versions 4.x de Moodle.

Si vous utilisez Moodle 3.x et que vous ne trouvez pas l'information dont vous avez besoin, consultez la rubrique [Dans le Moodle de votre établissement](/guide/creer-votre-classe-virtuelle/depuis-le-moodle-de-votre-etablissement.md) au bas de cette page. 
{% endhint %}

Après avoir cliqué sur l'activité BigBlueButton à l'étape précédente, vous arrivez sur la page de configuration de la salle.

**Principaux paramétrages**

Dans `Général`, vous pouvez :

* entrer le `Nom de la salle` (seul champ obligatoire)
* choisir le `Type de conférence` (avec ou sans enregistrement, ou `Enregistrement seulement` si aucune autre session n'est pas prévue et que vous souhaitez afficher uniquement les rediffusions).
* Une `Description` qui s'affichera en haut de l'activité.

![](/assets/moodle-ajout_bbb_general.png)

Les `Paramètres de la salle` permettent :

* d'afficher un `Message d'accueil` visible dans le chat de la classe virtuelle BBB (s'il est renseigné)
* d'afficher le message "La session peut être enregistrée" dans ce même chat (si coché)
* d'activer la salle d'attente de la classe virtuelle (si coché)

![](/assets/moodle4-plugin-param-salle.png)

Avec l'entrée `Réglages de verrouillage`, vous pouvez désactiver par défaut un certain nombre de fonctionnalités (webcam, micros, discussion privée, discussion publique et notes partagées) et masquer également la liste des participants.

![](/assets/moodle4-plugin-lock.png)

Via le menu déroulant de `Rôle attribué pendant la session en direct`, vous pouvez prédéfinir le statut (**participant** ou **modérateur**) qu'auront les inscrits au cours durant la classe virtuelle.

Vous pouvez choisir de les attribuer **par utilisateur** ou **par rôle d'inscription** au cours.

![Attribution du statut par utilisateur](/assets/moodle4-plugin-user-role.png)

![Attribution du statut par rôle](/assets/moodle4-plugin-role.png)

Vous pouvez aussi programmer une fenêtre d'affichage de votre salle dans le cours via le menu `Horaire de la réunion`.

![](/assets/moodle4-plugin-horaires.png)

**Lancer et animer la classe virtuelle**

A l'heure prévue, cliquez sur `Entrer dans la session` pour rejoindre la classe dans un nouvel onglet.

![](/assets/moodle4-plugin-ecran-lancement.png)

{% hint style="info" %}
Les parties 2 et 3 de ce guide concernent les fonctionnalités accessibles avec le LCMS Marsha et ne correspondent pas pour une utilisation avec le plugin BigBlueButton pour Moodle.

Pour un guide d'utilisation de BBB, rendez-vous directement sur la partie [Animer votre classe virtuelle](/guide/animer-votre-classe-virtuelle.md).
{% endhint %}

**Mettre fin à la classe virtuelle**

Avec le plugin BBB, l'interface est identique côtés enseignants et apprenants, à la différence du bouton `Terminer la session` qui permet à l'enseignant-modérateur de mettre fin à la session.

![](/assets/moodle4-plugin-fin.png)

Si la classe a été enregistrée, l'enregistrement apparaîtra au niveau du tableau des `Enregistrements`. Celui-ci sera accessible par défaut à tous les participants.

{% hint style="warning" %}
L'apparition du lien de téléchargement peut se faire en quelques minutes comme en plusieurs heures, en fonction de la durée de vos enregistrements.
{% endhint %}

Depuis cette interface, vous pouvez :

* Visionnez l'enregistrement (au format web)
* Modifier le nom et la description de la classe
* Rendre le partage public (en cliquant sur l'icône **cadenas**)
* Masquer l'enregistrement (en cliquant sur l'icone **œil**)
* Supprimer l'enregistrement (en cliquant sur l'icône **corbeille**)

![Tableau de récupération des enregistrements](/assets/moodle4-plugin-paramsalle.png)

#### Documentation complémentaire

* [La page du plugin BigBlueButtonBN](https://moodle.org/plugins/mod_bigbluebuttonbn) (en anglais) qui en propose une présentation en vidéo (en anglais).
* [La rubrique Moodle dans le centre d'aide de BigBlueButton](https://support.bigbluebutton.org/hc/en-us/categories/1500000533302-Moodle) (en anglais)
{% endtab %}
{% endtabs %}

[^1]: LTI (pour Learning Tools Interoperability) est une norme d’échange entre les outils d’apprentissage
