# Fiche Lou

**Version 0.2.15 · 2026-11-17 · Statut : premiers usages par la personne propriétaire.** Lou lit ses messages, e-mails et agenda, et n'envoie messages et e-mails qu'après validation de chacun.

## Rôle & limites
Une assistante personnelle : elle suit les engagements, prépare des réponses et des réunions, et garde le contexte des projets et du réseau de la personne qui l'utilise.
Elle **n'agit pas** d'elle-même, n'engage jamais sur de l'argent, des questions juridiques ou des accords, et n'interagit pas avec les personnes qui l'ont refusé. Liste complète : [principes](principles.fr.md).

## Autonomie
Aujourd'hui, **chaque message ou action qui touche une autre personne est validé** mot pour mot par la personne qui l'utilise avant d'avoir lieu.
Seule exception, qui ne concerne que la personne propriétaire : son propre agenda, pour des événements sans autre participant. Lou ajoute ou
déplace un événement à sa demande, et bloque d'elle-même un créneau que la personne propriétaire a accepté dans ses propres mots, ou une
réservation envoyée par une organisation (un train, un hôtel) ; si ses propres mots déplacent ou annulent ensuite ce créneau, Lou déplace ou
retire son blocage. Chaque changement est confirmé aussitôt, avec une annulation en un mot (niveau A3
ci-dessous). Le message d'une autre personne ne suffit jamais à rien changer. Tout changement est annoncé dans l'[historique](CHANGELOG.md).

## Ce que Lou sait faire
Généré à partir du registre des capacités de Lou : rien n'est mis en service sans une ligne ici.
- Répond à la personne propriétaire, prépare les brouillons et le point du matin (Anthropic, Claude).
- Tient un dossier par personne et organisation, regroupe les choses à faire en projets, sait où se trouve la personne propriétaire (Anthropic, Claude ; seulement des messages passés par la vérification).
- Vérifie chaque message pour en retirer les détails sensibles avant toute autre lecture, et permet une recherche par le sens (Mistral, UE).
- Transcrit les messages vocaux de la personne propriétaire (Mistral, UE) ; l'audio est supprimé une fois transcrit.
- Lit le texte des images et PDF que la personne propriétaire lui envoie (Mistral, UE), vérifié avant toute autre lecture ; le fichier est supprimé une fois lu.
- Cherche sur le web et lit des pages publiques pour des informations à jour (l'état d'un train, des horaires), via Anthropic ; jamais avec votre nom ou vos coordonnées, et chaque recherche et page est consignée.
- N'envoie un message ou un e-mail qu'après validation de ce texte exact par la personne propriétaire.
- Ajoute ou déplace des événements sans autre participant dans l'agenda de la personne propriétaire, bloque un créneau accepté ou une réservation, et déplace ou retire ses propres blocages quand ses mots les changent ; chaque fois annulable en un mot.

Pas encore : agir sur des sites web, envoyer dans des groupes, inviter des personnes à des événements.

## Modèles & données
| Rôle | Fournisseur |
|------|-------------|
| Vérification de confidentialité à l'arrivée : retire les détails sensibles avant que toute autre partie de Lou puisse lire un message ; recherche par le sens ; transcription des messages vocaux de la personne propriétaire, et texte des images et PDF qu'elle envoie | Mistral (UE) |
| Conversation, rédaction, et les dossiers (où en sont les choses avec chaque personne ou organisation, ce qui reste ouvert, chaque point avec ses messages), uniquement à partir de messages que la vérification a laissés passer ; recherches sur le web et pages publiques | Anthropic (Claude) |

Les données sont stockées sur des serveurs situés dans l'UE et sur les appareils de la personne propriétaire. Les fournisseurs d'IA ne reçoivent que les extraits nécessaires à chaque tâche.

## Données
- Jamais conservé : des notes ou profils contenant des informations sensibles sur les autres (santé, opinions politiques, religion, orientation sexuelle, origine ethnique, etc.). Lou garde un dossier par personne ou organisation (où en sont les choses, ce qui reste ouvert), rédigé uniquement à partir de messages vérifiés ; un point qu'aucun message ne prouve est refusé par le code.
- Un seul contrôle à l'arrivée : les détails sensibles concernant les autres sont retirés dès qu'un message arrive, et effacés de ce qui est enregistré ; d'ici là, aucune partie de Lou ne peut le lire. Les difficultés d'argent et les numéros de compte ou de carte sont traités de la même façon, y compris ceux de la personne propriétaire ; un prix ou une somme à rembourser reste.
- Appels : Lou sait quand la personne propriétaire a appelé quelqu'un qu'elle connaît déjà, et combien de temps, jamais ce qui s'est dit.
- Effacement : ce que vous avez écrit disparaît, et votre nom et vos coordonnées sont remplacés par « [erased] » partout où la personne propriétaire ou Lou les ont écrits.
- Une sauvegarde chiffrée de la base de données de Lou est faite chaque semaine et conservée 8 semaines sur les appareils de la personne propriétaire ; les données effacées en disparaissent dans ce délai.
- Lou garde une courte fiche contact par personne (nom, anniversaire, lien avec la personne propriétaire, contexte récent). Les liens avec la personne propriétaire et entre les personnes ne viennent que d'elle, jamais devinés.
- Lou regroupe aussi ce qu'elle sait par organisation (d'après les domaines des adresses e-mail) et par sujet récurrent. Les préférences de la personne propriétaire jouent seulement sur le style et les priorités : elles ne peuvent jamais donner une permission à Lou.
- Les contenus potentiellement sensibles sont scellés : chiffrés avec une clé que seule la personne propriétaire détient, Lou elle-même ne peut pas les lire *(en cours)*.
- Tous les détails : [politique de confidentialité](privacy-policy.fr.md).
- Ce que la personne propriétaire envoie à Lou : les messages vocaux sont transcrits et l'audio supprimé ; les images et PDF sont lus puis supprimés (au plus un jour) ; seul le texte est conservé. Tout ce qui n'est pas sa propre voix (un message transféré, une capture d'écran, un document) passe par la vérification de confidentialité avant toute autre lecture par une IA.
- Tout le monde est inclus par défaut et peut se retirer à tout moment, à l'un de ces trois niveaux :
  - **aucun contact** : Lou ne vous écrit jamais ;
  - **aucun contenu** : Lou sait seulement que vous avez écrit et quand, jamais quoi (aucune IA ne lit vos messages) ;
  - **ignorer** : Lou ne tient aucun compte de vos messages.
  Ce contrôle est fait par du code simple, avant toute intervention d'une IA.

## Niveaux de génération & d'autonomie
Chaque message préparé par Lou a une fiche de génération, disponible sur demande :

| Génération | | Décision | |
|-----------|--|----------|--|
| G0 | Écrit par la personne, sans IA | A1 | Écrit et envoyé par la personne |
| G1 | Corrigé ou traduit par Lou | A2 | Rédigé par Lou, relu et validé par la personne (par défaut) |
| G2 | Amélioré par Lou à partir de son texte | A3 | Fait par Lou sous une autorisation permanente (seulement l'agenda de la personne propriétaire : à sa demande, un créneau qu'elle a accepté, ou une réservation) |
| G3 | Généré à partir de consignes détaillées | | |
| G4 | Généré à partir d'une courte consigne | | |
| G5 | Généré sans consigne spécifique | | |

Les messages de niveau G2 et plus sont signés « Lou ». Les messages G0–G1 sont signés par la personne elle-même.
Un brouillon que la personne propriétaire envoie depuis son propre téléphone est son propre message et n'est pas signé Lou (par défaut, pour
les personnes qui lui sont proches) ; sa fiche de génération est conservée malgré tout, et disponible sur demande.

## Contact
**lou.kernel@gmail.com** (réponse personnelle de la personne propriétaire).
