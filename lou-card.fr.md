# Fiche Lou

**Version 0.2.6 · 2026-11-04 · Statut : premiers usages par la personne propriétaire.** Lou lit ses messages, e-mails et agenda, et n'envoie messages et e-mails qu'après validation de chacun.

## Rôle & limites
Une assistante personnelle : elle suit les engagements, prépare des réponses et des réunions, et garde le contexte des projets et du réseau de la personne qui l'utilise.
Elle **n'agit pas** d'elle-même, n'engage jamais sur de l'argent, des questions juridiques ou des accords, et n'interagit pas avec les personnes qui l'ont refusé. Liste complète : [principes](principles.fr.md).

## Autonomie
Aujourd'hui, **chaque message ou action qui touche une autre personne est validé** mot pour mot par la personne qui l'utilise avant d'avoir lieu.
Seule exception, qui ne concerne que la personne propriétaire : les changements dans son propre agenda qu'elle a demandés, sur des événements sans
autre participant, sont appliqués directement puis confirmés (niveau A3 ci-dessous). Tout changement est annoncé dans l'[historique](CHANGELOG.md).

## Modèles & données
| Rôle | Fournisseur |
|------|-------------|
| Conversation, rédaction, planification | Anthropic (Claude) |
| Vérification de confidentialité des messages (retire les détails sensibles), compréhension de ce qu'un message demande (pour prévenir) ; plus tard, transcription vocale | Mistral |

Les données sont stockées sur des serveurs situés dans l'UE et sur les appareils de la personne propriétaire. Les fournisseurs d'IA ne reçoivent que les extraits nécessaires à chaque tâche.

## Données
- Jamais conservé : des notes ou profils contenant des informations sensibles sur les autres (santé, opinions politiques, religion, orientation sexuelle, origine ethnique, etc.). Lou garde une courte note par conversation (où en sont les choses, ce qui reste à faire), rédigée à partir de messages déjà débarrassés des détails sensibles, puis vérifiée à nouveau.
- Les détails sensibles concernant les autres sont retirés automatiquement avant que l'IA de Lou ne lise un message, et effacés de ce qui est enregistré.
- Les contenus potentiellement sensibles sont scellés : chiffrés avec une clé que seule la personne propriétaire détient, Lou elle-même ne peut pas les lire *(en cours)*.
- Tous les détails : [politique de confidentialité](privacy-policy.fr.md).
- Lou ne garde aucune copie des enregistrements vocaux une fois transcrits.
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
| G2 | Amélioré par Lou à partir de son texte | A3 | Fait par Lou sous une autorisation permanente (seulement l'agenda de la personne propriétaire, à sa demande) |
| G3 | Généré à partir de consignes détaillées | | |
| G4 | Généré à partir d'une courte consigne | | |
| G5 | Généré sans consigne spécifique | | |

Les messages de niveau G2 et plus sont signés « Lou ». Les messages G0–G1 sont signés par la personne elle-même.

## Contact
**lou.kernel@gmail.com** (réponse personnelle de la personne propriétaire).
