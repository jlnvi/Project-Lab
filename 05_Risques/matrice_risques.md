# Matrice des risques — Équipe 1B Cybercore

> Project Lab ESIEE-IT · Sujet 2 : Interaction multimodale sécurisée
> Mise à jour à chaque revue de sprint.

## Échelle

- **Probabilité (P)** : 1 = faible · 2 = moyenne · 3 = forte
- **Impact (I)** : 1 = faible · 2 = moyen · 3 = fort
- **Criticité** = P × I : 1-2 faible · 3-4 moyenne · 6-9 **élevée**

## Matrice

| N° | Risque | Catégorie | P | I | Criticité | Prévention | Correction | Responsable | Statut |
|---|---|---|---|---|---|---|---|---|---|
| R1 | Usurpation d'une commande critique ou fuite de données personnelles | Sécurité | 2 | 3 | **6** | IA locale, authentification forte, chiffrement, journal infalsifiable | Révocation des accès, correctif, test de non-régression | Binôme Cyber | Ouvert |
| R2 | Projet jugé moins ambitieux sans robot physique | Projet | 2 | 3 | **6** | Ambition renforcée en Cyber et ILMSI, arbitrage documenté (DEC-05) | Démo du robot simulé + dossier sécurité | Chef de projet | Ouvert |
| R3 | Latence trop élevée de l'IA locale (> 5 s) | Technique | 2 | 3 | **6** | Petit modèle quantifié, réponses courtes, mesures dès le 1er sprint | Modèle plus léger, synthèse vocale en flux | Binôme ILMSI | Ouvert |
| R4 | Périmètre trop ambitieux (déjà vécu : humanoïde, robot physique) | Projet | 2 | 3 | **6** | MVP défini, priorités F1-F12, revue à chaque sprint | Couper les fonctions « souhaitables » | Chef de projet | Ouvert |
| R5 | Disponibilités réduites (alternance, équipe à 4) | Équipe | 3 | 2 | **6** | Travail à distance en période entreprise, tâches documentées | Réaffecter les tâches dans le binôme | Scrum master | Ouvert |
| R6 | Mauvaise compréhension du français par un petit modèle | Technique | 2 | 2 | 4 | Comparatif de modèles en phase de conception, prompt soigné | Essayer un modèle plus grand sur PC | Binôme ILMSI | Ouvert |
| R7 | Rejet de l'assistant par les seniors (gêne, méfiance) | Usage | 2 | 2 | 4 | Entretiens et questionnaire, voix lente et claire, pas de caméra | Ajuster la personnalité et les fonctions après les tests | Binôme ILMSI | Ouvert |
| R8 | Non-conformité RGPD (personnes vulnérables, données sensibles) | Juridique | 1 | 3 | 3 | Données minimisées, traitement local, consentement explicite | Suppression des données, revue RGPD | Binôme Cyber | Ouvert |
| R9 | Licence d'un modèle d'IA incompatible avec le projet | Juridique | 1 | 2 | 2 | Vérifier la licence avant chaque choix de modèle | Changer de modèle | Binôme ILMSI | Ouvert |
| R10 | Perte de code ou de travail | Équipe | 1 | 2 | 2 | GitHub, commits réguliers | Restauration depuis GitHub | Toute l'équipe | Ouvert |
| R11 | Départ du binôme RIT (compétences matériel) | Équipe | — | 3 | — | — | Traité par l'arbitrage DEC-05 (robot simulé) | — | **Clos** |

## Carte des risques

|  | **Impact faible (1)** | **Impact moyen (2)** | **Impact fort (3)** |
|---|---|---|---|
| **Probabilité forte (3)** | | R5 | |
| **Probabilité moyenne (2)** | | R6, R7 | R1, R2, R3, R4 |
| **Probabilité faible (1)** | | R9, R10 | R8 |

## Retours d'expérience

- **Humanoïde abandonné (DEC-02)** : un premier concept trop ambitieux nous a appris à définir un MVP et à revoir le périmètre régulièrement (R4).
- **Départ du binôme RIT (DEC-05)** : la perte d'une spécialité a montré qu'il faut documenter les tâches pour pouvoir les réaffecter (R5).
