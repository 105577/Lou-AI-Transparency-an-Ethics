# Politique de confidentialité

[English](privacy-policy.en.md) · Version 0.2.2 · 2026-11-04

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
- **Les messages envoyés au numéro WhatsApp de Lou.** Seuls ceux de la personne propriétaire sont traités. Si quelqu'un d'autre écrit à ce numéro, Lou enregistre
  seulement qu'un message est arrivé et quand, sans jamais le lire.

## Ce que Lou conserve

| Quoi | Pourquoi | Comment |
|------|----------|---------|
| Votre nom et vos coordonnées (numéro, adresse e-mail, identifiant de profil) tels qu'ils apparaissent dans les conversations de la personne propriétaire | Reconnaître la même personne d'une application à l'autre | Chiffrés ; retrouvés grâce à une empreinte à clé, jamais en clair |
| Les messages que vous échangez avec la personne propriétaire (pour les e-mails : objet et texte, sans les pièces jointes) | Rappeler à la personne propriétaire de répondre, aider à préparer réponses et rendez-vous | Chiffrés |
| Les messages rédigés par Lou, leur approbation par la personne propriétaire et leur envoi | Responsabilité : chaque message a une trace | Chiffrés, avec une empreinte qui révèle toute modification |
| Un journal d'activité : ce qui s'est passé et quand (identifiants, horaires, statuts, coûts) | Audits : tout ce que Lou a fait peut être retracé | **Ne contient aucun contenu de message.** Ne peut être ni modifié ni effacé, pas même par Lou |

**Jamais conservé :**
- des notes ou profils contenant des informations sensibles sur vous : santé, opinions politiques, religion, orientation sexuelle, origine ethnique,
  et informations similaires (pour l'instant, Lou ne rédige aucune note sur les personnes) ;
- **les détails sensibles de tes messages** : une vérification automatique, effectuée dans l'Union européenne, les retire avant que l'IA de Lou
  ne lise un message (« je ne pourrai pas venir demain, [raison personnelle] ») et les efface de la copie enregistrée. Si la vérification ne peut
  pas avoir lieu, le message est caché à Lou plutôt que lu ;
- les enregistrements vocaux, une fois transcrits ;
- quoi que ce soit venant des personnes ayant choisi le niveau **aucun contenu** ou **ignorer** (voir plus bas) : leurs messages sont écartés avant d'être enregistrés.

## Où, et qui d'autre y a accès

- **Stockage :** sur des serveurs situés dans l'**Union européenne**, et sur les appareils de la personne propriétaire. Le contenu est chiffré avec des clés détenues
  par la personne propriétaire ; l'hébergeur ne peut pas le lire.
- **Fournisseurs d'IA**, uniquement pour l'extrait nécessaire à une tâche donnée, jamais tout votre historique :
  - **Anthropic** (Claude), entreprise basée aux **États-Unis**, prépare les réponses et les brouillons. Selon ses conditions commerciales, ces données
    ne servent pas à entraîner ses modèles.
  - **Mistral**, basée dans l'**Union européenne**, pour la vérification qui retire les détails sensibles des messages ; plus tard, la transcription vocale. Elle ne reçoit que les messages qu'un premier jeu de règles signale comme possiblement sensibles.
- **Recherches sur le web :** pour des informations publiques et à jour (l'état d'un train, une entreprise, un lieu), Lou peut chercher sur le web
  via son fournisseur d'IA. Ces recherches portent sur des sujets publics : Lou a pour consigne de ne jamais y mettre votre nom ou vos coordonnées,
  et chaque recherche est enregistrée pour que la personne propriétaire puisse vérifier.
- **Les plateformes par lesquelles les messages passent déjà :** WhatsApp (Meta) pour le numéro de Lou, et Google pour les e-mails et l'agenda de la
  personne propriétaire, consultés via leurs interfaces officielles avec son autorisation.

Rien n'est vendu ni partagé à des fins publicitaires. Rien n'est publié.

## Combien de temps

- Conversations et brouillons : tant qu'ils sont utiles à la personne propriétaire, et jusqu'à ce que vous en demandiez l'effacement. Une durée maximale sera fixée
  et annoncée dans l'historique *(en cours)*.
- Enregistrements vocaux : supprimés une fois transcrits.
- Le journal d'activité : conservé, car c'est ce qui rend Lou vérifiable. Il ne contient aucun contenu de message.

## Les messages envoyés par Lou

Lou n'écrit à quelqu'un que lorsque la personne propriétaire a demandé ce message et approuvé le texte exact. Chaque message est signé **« Lou »** (le premier
renvoie ici), sauf s'il s'agit des propres mots de la personne propriétaire. Vous pouvez demander comment n'importe quel message a été rédigé : voir la
[fiche Lou](lou-card.fr.md).

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
efface ce qu'il ne permet plus.

**Comment le demander :** écrivez à **lou.kernel@gmail.com**, répondez à n'importe quel message signé Lou, ou dites-le directement à la personne propriétaire. Elle traite chaque demande personnellement :
les refus immédiatement, les autres demandes sous 30 jours. *(Les refus et effacements sont pour l'instant appliqués à la main par la personne propriétaire ;
leur automatisation est en cours.)*

Si vous résidez dans l'UE, vous disposez aussi des droits prévus par le RGPD, dont celui de saisir l'autorité de protection des données (en France, la CNIL).

## Sécurité

Contenu chiffré au repos ; un composant séparé, sans accès à l'IA, est le seul à pouvoir envoyer quoi que ce soit, et seulement les messages approuvés
par la personne propriétaire (vérifiés par une signature cryptographique) ; chaque étape est consignée dans un journal impossible à modifier. Le détail de
l'infrastructure n'est volontairement pas publié.

## Changements

Cette politique évolue avec Lou. Chaque version figure dans l'[historique](CHANGELOG.md), avec ce qui a changé et pourquoi.
