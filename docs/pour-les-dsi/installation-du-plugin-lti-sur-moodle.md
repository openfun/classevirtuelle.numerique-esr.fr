---
description: >-
  Installez l'outil de classes virtuelles en LTI sur le Moodle de votre
  établissement.
---

# Installer les classes virtuelles sur Moodle en LTI

La solution de classes virtuelles BBB est l'un des services proposés par le LCMS[^1] **Marsha** développé par France Université Numérique. Ce guide détaille la procédure d'installation des classes virtuelles en LTI mais peut aussi vous être utile si vous souhaitez utiliser les autres fonctionnalités disponibles : vidéo, webinaire, documents ou leçons au format Markdown[^2].

{% hint style="info" %}
L'installation du plugin LTI est compatible avec les versions 3.x et 4.x de Moodle
{% endhint %}

## **Prérequis**

{% hint style="warning" %}
Avant de vous rendre sur Moodle, vous devez obtenir **un passeport LTI** auprès de France Université Numérique en utilisant [ce formulaire de demande](https://www.fun-mooc.help/hc/fr/requests/new?ticket\_form\_id=9122250595357) ou en écrivant à l'adresse suivante : fun-ops\[a]fun-mooc.fr

Le passeport doit contenir 2 identifiants OAuth : une clef client[^3] et un secret partagé[^4].
{% endhint %}

## Ajouter un outil externe LTI

En étant connecté comme administrateur sur Moodle, accédez à l'`Administration du site` :

![](/assets/admin-moodle.png)

Rendez-vous sur l'onglet `Plugins`, puis cliquez sur `Gérer les outils` sous `Outils externes` :

![](/assets/moodle-outils.png)

### **Configuration semi-automatique**

Sur Moodle, il est possible d'ajouter un outil LTI Legacy préconfiguré. Une configuration supplémentaire sera néanmoins nécessaire (voir plus bas).

Pour ajouter cet outil, collez l'URL suivante `https://marsha.education/lti/config.xml` dans le champ `URL de l'outil...` et cliquez sur `Ajouter LTI Legacy`.

![](/assets/moodle-outils-legacy.png)

Un formulaire sera affiché <img src="/assets/key-secret.png" alt="Formulaire dans lequel saisir la clef et le secret" data-size="line">, demandant de renseigner les paramètres suivants :

| Champ          | Valeur                   |
| -------------- | ------------------------ |
| Clef client    | [dans le passeport LTI] |
| Secret partagé | [dans le passeport LTI] |

Remplissez-les avec les valeurs trouvées dans le passeport, puis cliquez sur `Enregistrer`.

Marsha sera disponible dans la liste des `Outils` :

![](/assets/marsha-outils.png)

### Configuration supplémentaire

Une configuration supplémentaire est nécessaire.

Cliquez sur la roue crantée <img src="/assets/moodle-outils-marsha-modifier.png" alt="" data-size="line"> sur l'outil Marsha, ce qui va ouvrir une page de `Configuration de l'outil externe` :

<figure><img src="/assets/moodle-config-additionnelle-v2.png" alt=""><figcaption><p>Les champs à modifier impérativement se trouvent dans la zone mise en évidence</p></figcaption></figure>

Remplissez le formulaire avec les données suivantes :

| Champ  |Valeur                       |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Utilisation de la configuration de l'outil | Afficher dans le sélecteur d'activité et comme outil préconfiguré   |
| Supporte les liens profonds   | Coché |
| URL de sélection de contenu   | `https://marsha.education/lti/select/classroom/` voir [A propos de l'URL de sélection de contenu](/pour-les-dsi/installation-du-plugin-lti-sur-moodle.md#warning-à-propos-de-lurl-de-sélection-de-contenu) |

### Customisation (facultatif)

#### Renommer l'outil

Pour rendre plus explicite l'accès pour les enseignants, vous pouvez modifier les champs `Nom de l'outil` en renseignant par exemple "**Classes virtuelles BBB"** et en modifiant la `Description de l'outil`.

![Exemple de renommage](/assets/moodle-config-outil-externe.png)

#### Modifier l'icône par défaut (facultatif)

Vous voudrez peut-être remplacer l'icône de l'outil LTI par celle-ci : <img src="/assets/favicon.ico" alt="" data-size="line">

Pour ce faire, cliquez sur `Afficher plus...` sous le champ URL de sélection de contenu.

![](/assets/moodle-config-afficher_plus.png)

Dans les 2 champs qui s'ouvrent, ajouter respectivement ces 2 URL :

| Champ                    | Valeur                                                |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| URL de l'icône           | `http://raw.githubusercontent.com/bigbluebutton/bigbluebutton/main/docs/static/img/favicon.ico`  |
|                          |                                                                                                                                                               |
| URL de l'icône sécurisée | ``https://raw.githubusercontent.com/bigbluebutton/bigbluebutton/main/docs/static/img/favicon.ico`|
|                          |                                                                                                                                                               |
|                          |                                                                                                                                                               |

![](/assets/moodle-config-ico-bbb.png)

L'icône de BigBlueButton sera affichée au niveau de l'outil configuré : <img src="/assets/moodle-custom-icon.png" alt="" data-size="line">

### Configuration des cookies

Les cookies sécurisés doivent être activés pour que l'authentification de réponse des liens profonds[^5] fonctionne.

S'ils ne sont pas activés sur votre instance, rendez-vous sur l'entrée `Sécurité HTTP` depuis Administration du site > Général > Sécurité et cochez la case `Cookies sécurisé uniquement` :

![](/assets/moodle4-custom-http.png)

### Redimensionnement automatique des iframes

Pour améliorer l'affichage et afin que les iframes soient toujours redimensionnées automatiquement, nous vous recommandons d'ajouter un script supplémentaire.

De retour dans la vue admin, onglet `Présentation`, cliquez sur `HTML additionnel` :

Collez le code suivant `Dans HEAD` et sauvegardez la page. `Within HEAD`:

```html
<script src="https://cdn.jsdelivr.net/npm/iframe-resizer@4.3.6/js/iframeResizer.min.js"></script>
<script>
    window.onload = function() {
        iFrameResize({checkOrigin: false}, '#contentframe');
    }
</script>
```

![](/assets/moodle-config-add-html.png)

### :warning: À propos de l'URL de sélection de contenu

{% hint style="warning" %}
Dans ce guide, nous vous proposons d'installer la solution de classes virtuelles BBB avec l'URL de sélection de contenu suivante :

`https://marsha.education/lti/select/classroom/`

L'utilisation de l'URL`https://marsha.education/lti/select/`vous permet au contraire d'intégrer par défaut toutes les ressources disponibles avec le LCMS Marsha.

Vous pouvez aussi, si vous le souhaitez, utiliser uniquement une ressource spécifique en la spécifiant dans l'URL de sélection de contenu. Pour cela, vous devez spécifier la ressource ciblée à la fin de l'URL.
{% endhint %}

<details>

<summary>Liste des ressources disponibles (services LTI proposés avec le LCMS Marsha)</summary>

**`video` : pour héberger et afficher des vidéos** :vhs:

```url
https://marsha.education/lti/select/video/
```

**`webinar` : pour organiser des webinaires** :movie\_camera:

```url
https://marsha.education/lti/select/webinar/
```

**`document` : pour héberger et partager des fichiers** :open\_file\_folder:

```url
https://marsha.education/lti/select/document/
```

**`classroom` : pour organiser des classes virtuelles avec BigBlueButton** :sparkles:

```url
https://marsha.education/lti/select/classroom/
```

**`markdown` : pour créer de leçons au format Markdown** :writing\_hand:

```url
https://marsha.education/lti/select/markdown/
```

**`deposit` : pour collecter des devoirs** :card\_box:

```url
https://marsha.education/lti/select/deposit/
```

</details>

Une fois l'outil configuré avec cette URL spécifique, il suffira de l'ajouter dans le cours pour obtenir uniquement le contenu relatif à cette ressource.

## Utilisation de Moodle par les enseignants

L'outil externe est configuré, les enseignants peuvent l'utiliser ! :tada:

Ce guide est à leur disposition : [Créer votre classe virtuelle depuis le Moodle de votre établissement](/guide/creer-votre-classe-virtuelle/depuis-le-moodle-de-votre-etablissement.md)

[^1]: Gestionnaire de contenus pour l'éducation (ou Learning Content Management System)

[^2]: Markdown est un langage de balisage léger qui permet de formater du texte de manière simple et rapide

[^3]: consumer key

[^4]: shared secret

[^5]: Un "deeplink" est un lien spécifique visant à renvoyer vers une page ou un produit précis, au lieu de rediriger uniquement vers la page d’accueil de l’application.
