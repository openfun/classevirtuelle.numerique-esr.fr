---
description: Installez ou activez le plugin BBB dans le Moodle de votre établissement
---

# Intégrer le plugin BBB sur Moodle

[Blindside Networks](https://blindsidenetworks.com/), l'éditeur du logiciel libre BigBlueButton, a développé un plugin BBB pour Moodle. Dans le cadre du Plan de relance, [France Université Numérique](https://www.france-universite-numerique.fr/) délivre des identifiants d'un serveur dédié à l'ESR et opéré par [Arawa](https://www.arawa.fr/) afin de permettre aux enseignants de réaliser des classes virtuelles sans connaître les limitations de la version d'essai.

## **Prérequis**

{% hint style="warning" %}
Avant de vous rendre sur Moodle, vous devez obtenir les identifiants du serveur BigBlueButton auprès de France Université Numérique en utilisant [ce formulaire de demande](https://www.fun-mooc.help/hc/fr/requests/new?ticket\_form\_id=9122250595357) ou en écrivant à l'adresse suivante : fun-ops\[a]fun-mooc.fr.

Une version de test est néanmoins fonctionnelle sur Moodle 4.x pour expérimenter la solution avant de l'installer.
{% endhint %}

## Installer le plugin BigBlueButton sur Moodle 3.x

{% hint style="info" %}
Le plugin BigBlueButton est intégré par défaut [depuis la version 4.0 de Moodle](https://bigbluebutton.org/2022/04/19/bigbluebutton-your-online-teaching-advantage-now-fully-integrated-into-moodle/).

Pour les versions 3.x de Moodle, il vous faut intégrer le plugin **BigBlueButtonBN**.
{% endhint %}

Téléchargez le plugin qui correspond à votre version de Moodle depuis cette page :

{% embed url="https://moodle.org/plugins/pluginversions.php?plugin=mod_bigbluebuttonbn" %}

Le guide d'installation de plugins sur Moodle se trouve ici :

{% embed url="https://docs.moodle.org/4x/fr/Installation_de_plugins" %}

Le code source et les recommandations pour l'installation de BigBlueButton :

{% embed url="https://github.com/blindsidenetworks/moodle-mod_bigbluebuttonbn" %}
Code source et guide d'installation du logiciel
{% endembed %}

## Activer le plugin BigBlueButton sur Moodle 4.x

Sur les versions 4.x de Moodle, il ne suffit que d'activer le plugin BBB préinstallé pour rendre accessible les classes virtuelles aux enseignants.

### Configurer le plugin

Dans `Administration du site`, choisissez l'onglet `Plugins` :

![](/assets/moodle4-plugins.png)

Choisissez l'entrée `Gestion des activités` dans la rubrique `Modules d'activité` :

![](/assets/moodle4-gestion-activites.png)

![](/assets/moodle4-params-bbb.png)

Pour activer le plugin, vous devez donner votre accord au traitement des données par l'éditeur du logiciel Blindside Networks puis renseigner les identifiants fournis par France Université Numérique :

* `URL du serveur BigBlueButton`
* `Secret partagé BigBlueButton`

![](/assets/moodle4-plugin-reglages.png)

{% hint style="info" %}
Si vous souhaitez expérimenter la solution avant de contacter FUN, vous pouvez utiliser le serveur de test mis à disposition par Blindside Networks pour lequel les identifiants sont préremplis.

Prêtez alors attention aux limitations énumérées sur la page (voir image ci-dessus).
{% endhint %}

### Afficher le plugin dans les activités de cours

Une fois la configuration achevée, retournez sur la page `Gestion des activités`.

Sur la ligne BigBlueButton, cliquez sur l'icône en forme d’œil pour afficher le plugin.

![](/assets/moodle4-plugin-afficher.png)

Le plugin est désormais fonctionnel ! :tada:

Vous pouvez renvoyez les enseignants vers le guide d'utilisation suivant : [Créer votre classe virtuelle depuis le Moodle de votre établissement](/guide/creer-votre-classe-virtuelle/depuis-le-moodle-de-votre-etablissement.md)
