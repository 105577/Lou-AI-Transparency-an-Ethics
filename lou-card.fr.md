# Fiche Lou

**Version 0.1.1 · 2026-10-28 · Statut : en développement, pas encore en service.**

## Rôle & limites
Une assistante personnelle : elle suit les engagements, prépare des réponses et des réunions, et garde le contexte des projets et du réseau de la personne qui l'utilise.
Elle **n'agit pas** d'elle-même, n'engage jamais sur de l'argent, des questions juridiques ou des accords, et n'interagit pas avec les personnes qui l'ont refusé. Liste complète : [principes](principles.fr.md).

## Autonomie
Aujourd'hui, **chaque message ou action sortant est validé** par la personne qui l'utilise avant d'avoir lieu. Tout changement est annoncé dans l'[historique](CHANGELOG.md).

## Modèles & données
| Rôle | Fournisseur |
|------|-------------|
| Conversation, rédaction, planification | Anthropic (Claude) |
| Transcription vocale, indexation, petites tâches de classification | Mistral |

Les données sont stockées sur des serveurs situés dans l'UE et sur les appareils de la personne propriétaire. Les fournisseurs d'IA ne reçoivent que les extraits nécessaires à chaque tâche.

## Données
- Jamais conservé : les informations sensibles sur les autres (santé, opinions politiques, religion, orientation sexuelle, origine ethnique, etc.).
- Les contenus potentiellement sensibles sont scellés : chiffrés avec une clé que seule la personne propriétaire détient, Lou elle-même ne peut pas les lire.
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
| G2 | Amélioré par Lou à partir de son texte | A3 | Envoyé par Lou sous une autorisation permanente (non utilisé) |
| G3 | Généré à partir de consignes détaillées | | |
| G4 | Généré à partir d'une courte consigne | | |
| G5 | Généré sans consigne spécifique | | |

Les messages de niveau G2 et plus sont signés « Lou ». Les messages G0–G1 sont signés par la personne elle-même.

## Contact
**lou@…** (réponse personnelle de la personne propriétaire).
