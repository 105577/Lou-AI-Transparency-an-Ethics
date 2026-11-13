# Politique de confidentialité

[English](privacy-policy.en.md) · Version 0.2.13 · 2026-11-13

Lou est l'assistante IA personnelle d'une personne, publiée ici sous le pseudonyme **115** (« la personne propriétaire »).
Cette page dit simplement ce que Lou lit, ce qu'elle conserve, où, combien de temps, qui d'autre y a accès, et comment vous pouvez le limiter ou l'effacer.
Elle décrit Lou **telle qu'elle fonctionne aujourd'hui**. Ce qui est encore en construction est indiqué *(en cours)*. Chaque changement est consigné
dans l'[historique](CHANGELOG.md).

## Qui est responsable

La personne propriétaire. Lou est un outil personnel, pas une entreprise ni un service proposé au public. Elle n'est pas vendue, ne contient aucune publicité
et ne constitue de profil sur personne pour le compte de qui que ce soit. La personne propriétaire répond personnellement à chaque demande concernant vos données
(voir [Vos choix](#vos-choix)).

## Ce que Lou lit

Uniquement ce qui parvient à la personne propriétaire, avec son autorisation :

- **Les conversations de la personne propriétaire** sur ses messageries (par exemple WhatsApp, LinkedIn, Instagram, Messenger, iMessage), lues par une application
  installée sur l'ordinateur de la personne propriétaire. En lecture seule, sauf pour les messages que la personne propriétaire a approuvés un par un.
- **Les e-mails de la personne propriétaire** : pour chaque e-mail, l'expéditeur, les destinataires, la date, l'objet, son texte et son identifiant technique.
  **Les pièces jointes ne sont jamais ouvertes.**
- **L'agenda de la personne propriétaire** : titres, horaires, lieux et nombre de participants des événements.
- **Les appels téléphoniques de la personne propriétaire**, depuis l'historique d'appels de son propre ordinateur : avec qui, quand, dans quel sens,
  s'il a été décroché et combien de temps. **Jamais ce qui s'est dit.** Seulement les appels avec des personnes que Lou connaît déjà par les
  messages de la personne propriétaire ; un appel n'ajoute jamais personne.
- **Les contacts de la personne propriétaire**, seulement quand elle les exporte pour Lou : noms, numéros et adresses, pour mettre un nom sur des
  personnes que Lou connaît déjà. Lou n'y ajoute personne et n'a aucun accès permanent à son carnet d'adresses.
- **Les messages envoyés au numéro WhatsApp de Lou.** Seuls ceux de la personne propriétaire sont traités. Si quelqu'un d'autre écrit à ce numéro, Lou enregistre
  seulement qu'un message est arrivé et quand, sans jamais le lire.

## Ce que Lou conserve

| Quoi | Pourquoi | Comment |
|------|----------|---------|
| Votre nom et vos coordonnées (numéro, adresse e-mail, identifiant de profil) tels qu'ils apparaissent dans les conversations de la personne propriétaire | Reconnaître la même personne d'une application à l'autre | Chiffrés ; retrouvés grâce à une empreinte à clé, jamais en clair ; deux fiches au même nom complet sont traitées comme une seule personne, et la personne propriétaire peut les séparer |
| Les messages que vous échangez avec la personne propriétaire (pour les e-mails : objet et texte, sans les pièces jointes) | Rappeler à la personne propriétaire de répondre, aider à préparer réponses et rendez-vous | Chiffrés |
| Vos appels avec la personne propriétaire : quand, dans quel sens, combien de temps | Que Lou sache qu'une chose a pu se régler au téléphone, et demande à la personne propriétaire plutôt que de deviner | Jamais ce qui s'est dit ; seulement si Lou vous connaît déjà ; effacés avec vos données sur demande |
| Un dossier par personne ou organisation : où en sont les choses, et ce qui reste ouvert entre vous et la personne propriétaire (une chose à faire, une chose attendue, une date convenue), chaque point avec les messages dont il vient | Éviter à la personne propriétaire de tout relire, sans rien oublier ni inventer | Chiffré ; rédigé uniquement à partir de messages que la vérification de confidentialité a laissés passer ; un point qu'aucun message ne prouve est refusé par le code ; corrigeable par la personne propriétaire, et Lou lui pose la question quand elle ne peut pas savoir (un appel, une rencontre) ; effacé au bout de 12 mois, ou avec vos données sur demande |
| Une fiche contact à votre sujet : votre nom et vos surnoms, votre anniversaire, votre lien avec la personne propriétaire et votre degré de proximité, votre travail, comment vous vous êtes rencontrés, une description en une ligne, et le contexte récent | Que Lou sache qui vous êtes quand vous écrivez, sans avoir à chercher | Chiffrée ; votre lien avec la personne propriétaire, votre degré de proximité et les liens entre personnes ne viennent que de la personne propriétaire, jamais devinés ; jamais d'informations sensibles ; effacée avec vos données sur demande |
| L'organisation depuis laquelle vous écrivez, trouvée d'après le domaine de votre adresse e-mail (jamais une messagerie gratuite comme Gmail), votre rôle si la personne propriétaire l'indique, et les sujets dont vous parlez avec elle dès qu'ils reviennent dans plus d'une conversation | Qu'un nouveau message arrive avec son historique, même depuis une autre adresse de la même organisation | Chiffrés ; domaines conservés sous forme d'empreintes à clé, jamais en clair ; jamais d'informations sensibles ; votre lien à une organisation est effacé avec vos données sur demande |
| Les préférences de la personne propriétaire à votre sujet (par exemple « toujours en français ») | Que Lou suive la façon de faire de la personne propriétaire | Chiffrées ; uniquement de la personne propriétaire, jamais de vos messages ; elles ne peuvent jamais donner une permission à Lou ; effacées avec vos données sur demande |
| Un journal de chaque modification de ce que Lou sait (quoi, d'où, par qui) | Pouvoir expliquer et annuler chaque modification | Chiffré ; impossible à réécrire ; son contenu est effacé au bout de 12 mois, ou avec vos données sur demande |
| De courts faits que Lou apprend, sur vous ou sur la personne propriétaire (où vous travaillez, une préférence, un projet), chacun avec sa source ; et ce qu'il y avait à faire entre vous et la personne propriétaire, et comment cela s'est terminé | Que Lou se souvienne de ce qui compte et ne signale pas deux fois la même chose | Chiffrés ; jamais d'informations sensibles ; les faits appris de vos messages sont listés à la personne propriétaire, qui peut les corriger ou les retirer ; effacés au bout de 12 mois, ou avec vos données sur demande |
| Un index de recherche de ce que Lou conserve : des empreintes de mots et des vecteurs de « sens » | Permettre à la personne propriétaire de tout retrouver en demandant (« qu'a dit Clara sur la présentation ? ») | Construit uniquement à partir de textes débarrassés des détails sensibles ; les mots sont enregistrés sous forme d'empreintes à clé, jamais en clair ; vecteurs chiffrés ; rien des personnes qui ont refusé ; effacé avec le contenu |
| Les messages rédigés par Lou, leur approbation par la personne propriétaire et leur envoi | Responsabilité : chaque message a une trace | Chiffrés, avec une empreinte qui révèle toute modification |
| Un journal d'activité : ce qui s'est passé et quand (identifiants, horaires, statuts, coûts) | Audits : tout ce que Lou a fait peut être retracé | **Ne contient aucun contenu de message.** Ne peut être ni modifié ni effacé, pas même par Lou |

**Jamais conservé :**
- des notes ou profils contenant des informations sensibles sur vous : santé, opinions politiques, religion, orientation sexuelle, origine ethnique,
  ennuis judiciaires, crises de couple et informations similaires (les dossiers de Lou ne sont rédigés qu'à partir de messages vérifiés, et vérifiés
  de nouveau quand les règles s'élargissent) ;
- **les détails sensibles de vos messages** : une vérification automatique, effectuée dans l'Union européenne, les retire **dès qu'un message
  arrive, avant que quoi que ce soit d'autre dans Lou puisse le lire** (« je ne pourrai pas venir demain, [raison personnelle] »), et les efface de
  la copie enregistrée. Tant que la vérification n'a pas laissé passer un message, aucune partie de Lou ne peut le lire ; si elle ne peut pas avoir
  lieu, le message attend, sans être lu, et il est vérifié de nouveau plus tard. Cela inclut les **difficultés d'argent**, y compris celles de la
  personne propriétaire (un découvert, une dette, une perte, un recouvrement) et les numéros de compte ou de carte, remplacés par
  « [information financière] » ; un prix ou une somme à payer ou à rembourser n'est pas sensible et reste ;
- les enregistrements vocaux, une fois transcrits ;
- quoi que ce soit venant des personnes ayant choisi le niveau **aucun contenu** ou **ignorer** (voir plus bas) : leurs messages sont écartés avant d'être enregistrés.

## Où, et qui d'autre y a accès

- **Stockage :** sur des serveurs situés dans l'**Union européenne**, et sur les appareils de la personne propriétaire. Le contenu est chiffré avec des clés détenues
  par la personne propriétaire ; l'hébergeur ne peut pas le lire.
- **Fournisseurs d'IA**, uniquement pour l'extrait nécessaire à une tâche donnée, jamais tout votre historique :
  - **Mistral**, basée dans l'**Union européenne**, effectue la vérification de confidentialité : c'est le filtre entre le monde et le reste de
    Lou. Elle ne reçoit que les messages qu'un premier jeu de règles signale. Elle permet aussi à la recherche de Lou de comprendre le sens
    (« l'appartement » trouve aussi « l'appart ») ; plus tard, la transcription vocale.
  - **Anthropic** (Claude), entreprise basée aux **États-Unis**, prépare les réponses et les brouillons, et tient les dossiers (où en sont les
    choses avec chaque personne ou organisation, ce qui reste ouvert, chaque point avec ses messages). Elle ne lit un message **qu'une fois que la
    vérification de confidentialité l'a laissé passer**, jamais avant. Selon ses conditions commerciales, ces données ne servent pas à entraîner
    ses modèles.
- **Recherches sur le web :** pour des informations publiques et à jour (l'état d'un train, une entreprise, un lieu), Lou peut chercher sur le web
  via son fournisseur d'IA. Ces recherches portent sur des sujets publics : Lou a pour consigne de ne jamais y mettre votre nom ou vos coordonnées,
  et chaque recherche est enregistrée pour que la personne propriétaire puisse vérifier.
- **Les plateformes par lesquelles les messages passent déjà :** WhatsApp (Meta) pour le numéro de Lou, et Google pour les e-mails et l'agenda de la
  personne propriétaire, consultés via leurs interfaces officielles avec son autorisation.

Rien n'est vendu ni partagé à des fins publicitaires. Rien n'est publié.

## Combien de temps

- Messages, e-mails, brouillons et échanges de la personne propriétaire avec Lou : leur **texte est effacé automatiquement au bout de 12 mois**,
  ou plus tôt si vous le demandez. Il reste un enregistrement sans contenu (qui a écrit, quand, si un message a été envoyé, et une empreinte
  qui prouve ce qui a été envoyé sans permettre de le relire), conservé avec le journal d'activité.
- Les dossiers et le journal des modifications de ce que Lou sait : leur texte est lui aussi effacé au bout de 12 mois.
- Enregistrements vocaux : supprimés une fois transcrits.
- Le journal d'activité : conservé **3 ans**, car c'est ce qui rend Lou vérifiable. Il ne contient aucun contenu de message.
- Sauvegardes : une copie chiffrée de la base de données de Lou chaque semaine, sur les appareils de la personne propriétaire ; les
  **8 dernières semaines** sont conservées. Ce qui est effacé (sur demande ou au bout de 12 mois) disparaît des sauvegardes à mesure
  qu'elles sont remplacées, en 8 semaines au plus. Les sauvegardes ne servent qu'à restaurer Lou après une panne.

## Les messages envoyés par Lou

Lou n'écrit à quelqu'un que lorsque la personne propriétaire a demandé ce message et approuvé le texte exact. Chaque message est signé **« Lou »** (le premier
renvoie ici), sauf s'il s'agit des propres mots de la personne propriétaire. Vous pouvez demander comment n'importe quel message a été rédigé : voir la
[fiche Lou](lou-card.fr.md).

Lou peut aussi préparer un message que la personne propriétaire envoie ensuite **depuis son propre téléphone, comme son propre message** ; par
défaut, pour les personnes qui lui sont proches. Un tel message n'est pas signé Lou, puisque c'est la personne propriétaire qui l'envoie ; la
façon dont il a été rédigé (et la part de Lou) est enregistrée malgré tout, et vous pouvez la demander pour n'importe quel message reçu d'elle.

## Vos choix

Tout le monde commence au niveau **complet**. Vous pouvez changer de niveau à tout moment ; le changement s'applique dès que la personne propriétaire reçoit votre
demande, et il est vérifié par du code simple, avant toute intervention d'une IA :

| Niveau | Lou vous écrit | Lou conserve vos messages | Une IA lit vos messages |
|--------|:---:|:---:|:---:|
| **complet** (par défaut) | ✓ (approuvé par la personne propriétaire) | ✓ chiffrés | ✓ |
| **aucun contact** | ✗ | ✓ chiffrés | ✓ |
| **aucun contenu** | ✗ | seulement que vous avez écrit, et quand | ✗ |
| **ignorer** | ✗ | ✗ | ✗ |

La personne propriétaire peut aussi, de sa propre initiative, appliquer l'un de ces niveaux à quelqu'un, ou demander à Lou de ne jamais lire les
e-mails d'un domaine donné (par exemple un cabinet médical). Vous pouvez aussi demander à la personne propriétaire de **consulter** ce que Lou détient sur vous, de le **corriger** ou de l'**effacer**. Baisser votre niveau
efface ce qu'il ne permet plus *(en cours : pour l'instant, demandez aussi l'effacement)*.

**Comment le demander :** écrivez à **lou.kernel@gmail.com**, répondez à n'importe quel message signé Lou, ou dites-le directement à la personne propriétaire. Si vous demandez dans un message à ne plus être contacté par Lou ou à ce qu'aucune IA ne lise vos messages, Lou l'enregistre comme une demande et prévient aussitôt la personne propriétaire. Elle traite chaque demande personnellement :
les refus immédiatement, les autres demandes sous 30 jours. Chaque demande est enregistrée avec son échéance et suivie jusqu'à sa réponse.
Un effacement est préparé par Lou et ne s'exécute qu'une fois approuvé par la personne propriétaire ; il supprime le texte de vos messages,
votre nom et vos coordonnées, et ne garde qu'une trace : que des messages ont existé, et quand, avec vos coordonnées sous forme d'empreintes
illisibles, pour que vos choix continuent de s'appliquer. Partout où la personne propriétaire ou Lou ont écrit votre nom ou vos coordonnées (les
propres messages de la personne propriétaire à Lou, ses rappels, ses choses à faire, les journaux de Lou), ils sont remplacés par « [erased] » :
les traces restent, sans vous.

Si vous résidez dans l'UE, vous disposez aussi des droits prévus par le RGPD, dont celui de saisir l'autorité de protection des données (en France, la CNIL).

## Sécurité

Contenu chiffré au repos ; un composant séparé, sans accès à l'IA, est le seul à pouvoir envoyer quoi que ce soit, et seulement les messages approuvés
par la personne propriétaire (vérifiés par une signature cryptographique) ; chaque étape est consignée dans un journal impossible à modifier. Le détail de
l'infrastructure n'est volontairement pas publié.

## Changements

Cette politique évolue avec Lou. Chaque version figure dans l'[historique](CHANGELOG.md), avec ce qui a changé et pourquoi.
