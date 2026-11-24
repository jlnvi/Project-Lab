# Impacts, DD&RS et RGPD — Équipe 1B Cybercore

> Project Lab ESIEE-IT · Sujet 2 : Interaction multimodale sécurisée
> Objectif : analyser les impacts positifs et négatifs du projet, et montrer comment ils influencent nos choix.

## 1. Impacts positifs

| Impact | Pour qui |
|---|---|
| Moins d'isolement : une présence qui parle et écoute | Personnes âgées |
| Plus de sorties et de contacts : l'assistant propose de sortir ou d'appeler un proche | Personnes âgées |
| Autonomie à domicile : rappels du quotidien sans dépendre d'un écran | Personnes âgées |
| Aidants rassurés, charge mentale réduite | Aidants |
| Une alternative qui protège la vie privée face aux assistants cloud | Société |

## 2. Impacts négatifs et nos choix

| Impact négatif possible | Notre choix pour le limiter | Où c'est traduit |
|---|---|---|
| L'assistant remplace le lien humain | Il pousse à sortir et à appeler un proche, il ne se présente pas comme un ami de substitution | F6, objectif O2 |
| Sentiment d'être surveillé | Micro activé seulement par le mot d'éveil, pas de caméra dans le prototype (si ajoutée plus tard : voyant visible et images traitées en local), avatar qui montre clairement quand il écoute | F1, F5 |
| L'aidant « espionne » son proche | L'aidant ne lit pas les conversations, seulement les messages et rappels qu'il gère | S7 |
| Exclusion des personnes peu à l'aise avec le numérique | Tout se fait à la voix ; l'appli est pour l'aidant | F1 à F4 |
| Usurpation, arnaque, prise de contrôle | Commandes critiques authentifiées et tracées | F8, F9, S2 à S4 |
| Dépendance à un fournisseur ou à un abonnement | Briques open source, IA locale, pas d'abonnement | DEC-04 |
| Empreinte environnementale | Aucun matériel neuf : tout tourne sur des PC existants ; pas de serveurs cloud | DEC-05 |

## 3. DD&RS

| Dimension | Ce que fait le projet |
|---|---|
| **Environnement** | Pas de matériel neuf (robot simulé, PC existants), pas de serveur cloud qui tourne en continu, petits modèles d'IA quantifiés moins gourmands |
| **Social** | Lutte contre l'isolement des seniors ; tests avec de vrais utilisateurs ; interface pensée pour les personnes peu à l'aise avec le numérique |
| **Éthique** | L'assistant ne se fait pas passer pour un humain ; respect de l'intimité vis-à-vis des aidants ; pas de suivi médical ni de diagnostic |
| **Ouverture** | Briques open source, code versionné sur GitHub, documentation reproductible |

## 4. RGPD

Le projet concerne des **personnes vulnérables** (personnes âgées isolées) et peut toucher des informations sur leur moral ou leur santé. La protection des données est donc un enjeu central.

### Données traitées

| Donnée | Pourquoi | Où | Durée de conservation |
|---|---|---|---|
| Voix de l'utilisateur | Comprendre la demande | PC du domicile, en mémoire | Non conservée après transcription |
| Transcription et réponses | Dialoguer, contexte court | PC du domicile | Fin de la conversation [À COMPLÉTER : durée] |
| Rappels et messages de l'aidant | Fonction rappels et messages | PC du domicile, base chiffrée | Jusqu'à suppression par l'aidant |
| Compte de l'aidant | Authentification | PC du domicile, base chiffrée | Durée d'utilisation du service |
| Journal des commandes critiques | Traçabilité, sécurité | PC du domicile, base chiffrée | [À COMPLÉTER : ex. 6 mois] |

### Principes appliqués

- **Minimisation** : on ne collecte que ce qui sert une fonction ; la voix n'est pas conservée.
- **Traitement local** : aucune donnée n'est envoyée sur Internet (exigence S1).
- **Consentement** : explicite, recueilli auprès de la personne âgée avant la mise en service.
- **Droits** : la personne peut consulter et supprimer ses données (effacement).
- **Sécurité** : chiffrement, authentification, journal (exigences S2 à S6).
- **Analyse d'impact (AIPD)** : à évaluer, car le traitement concerne des personnes vulnérables.

### Pendant le projet (entretiens, questionnaire, tests)

- Questionnaire anonyme, adresse e-mail non collectée.
- Entretiens anonymisés : aucun nom ni photo publié, consentement oral recueilli.
- Tests utilisateurs : consentement recueilli, résultats anonymisés.
