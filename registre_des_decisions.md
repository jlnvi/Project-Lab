# Registre des décisions — Équipe 1B Cybercore

> Project Lab ESIEE-IT · Sujet 2 : Interaction multimodale sécurisée
> Ce registre trace chaque décision structurante du projet : le contexte, les options étudiées, le choix retenu et sa justification.
> Les éléments entre `[À COMPLÉTER]` sont à renseigner par l'équipe.

| N° | Date | Décision | Statut |
|---|---|---|---|
| DEC-01 | [À COMPLÉTER] | Choix du sujet 2 « Interaction multimodale sécurisée » | Validée (Commission 1, 21/10/2026) |
| DEC-02 | [À COMPLÉTER] | Abandon du robot humanoïde au profit d'un robot fixe | Validée |
| DEC-03 | [À COMPLÉTER] | Recentrage : abandon de la reconnaissance de gestes | Validée |
| DEC-04 | [À COMPLÉTER] | IA 100 % locale plutôt qu'un service cloud | Validée |
| DEC-05 | [À COMPLÉTER] | Robot physique remplacé par un robot simulé, tout sur PC | Validée |

---

## DEC-01 — Choix du sujet 2

- **Date :** [À COMPLÉTER]
- **Participants :** Julien, Ajanthan, Donald, Jedcy (+ binôme RIT à l'époque)
- **Contexte :** l'équipe mixte (Cyber, ILMSI, RIT) devait choisir un sujet parmi ceux proposés pour le Project Lab.
- **Décision :** sujet 2, « Interaction multimodale sécurisée » : piloter un robot par plusieurs modes d'interaction (voix, geste, application), de façon sécurisée.
- **Justification :** sujet qui mobilise chaque spécialité de l'équipe ; la sécurité y est centrale, ce qui valorise le binôme Cyber.
- **Validation :** Commission 1 du 21/10/2026.

## DEC-02 — Robot humanoïde → robot fixe

- **Date :** [À COMPLÉTER]
- **Participants :** [À COMPLÉTER]
- **Contexte :** le premier concept était un robot humanoïde qui préparait les repas de personnes âgées.
- **Options étudiées :**
  1. Garder l'humanoïde (mobilité + manipulation d'objets)
  2. Robot fixe de bureau ou de maison, qui ne se déplace pas
- **Décision :** option 2, robot fixe.
- **Justification :** la mobilité et la manipulation d'objets sont irréalisables avant la soutenance d'avril, avec nos compétences et notre temps. L'effort est reporté sur l'interaction et la sécurité, qui sont le cœur du sujet.
- **Conséquences :** déplacement, bras et préparation de repas passent hors périmètre.

## DEC-03 — Abandon de la reconnaissance de gestes

- **Date :** [À COMPLÉTER] (après la Commission 1)
- **Participants :** [À COMPLÉTER]
- **Contexte :** retour du jury en Commission 1 : « centrer notre solution », argumenter nos choix, analyser l'existant.
- **Options étudiées :**
  1. Voix + gestes + application (projet large)
  2. Voix + application pour les aidants (projet centré)
- **Décision :** option 2. La voix est le mode principal pour l'utilisateur âgé ; l'application sert à l'aidant. Le projet reste multimodal.
- **Justification :** les gestes dispersaient l'effort sans apport clair pour la cible ; la voix est le mode le plus naturel pour une personne âgée peu à l'aise avec le numérique.
- **Conséquences :** la reconnaissance de gestes passe hors périmètre.

## DEC-04 — IA 100 % locale plutôt que cloud

- **Date :** [À COMPLÉTER]
- **Participants :** [À COMPLÉTER]
- **Contexte :** l'assistant doit comprendre et répondre à la voix. Les assistants du marché (Alexa, Google Home) traitent la voix dans le cloud.
- **Options étudiées :**
  1. API cloud (simple, performante, mais la voix quitte le domicile)
  2. Modèles open source exécutés en local (whisper.cpp, petit LLM, Piper TTS)
- **Décision :** option 2, traitement 100 % local.
- **Justification :** confidentialité des conversations d'une personne vulnérable (RGPD), fonctionnement hors ligne, et c'est notre différence face à l'existant.
- **Conséquences :** risque de latence à surveiller (critère : réponse en moins de 5 s) ; licences des modèles à vérifier.

## DEC-05 — Robot physique → robot simulé, tout sur PC

- **Date :** [À COMPLÉTER]
- **Participants :** Julien, Ajanthan, Donald, Jedcy
- **Contexte :** le binôme RIT (Yoann, Antoine) a quitté l'équipe. Les compétences matériel (électronique, servos, impression 3D, réseau) sont parties avec lui. L'équipe passe de 6 à 4 personnes.
- **Options étudiées :**
  1. Construire quand même le robot physique (Raspberry Pi 5, servos, boîtier imprimé en 3D)
  2. Robot simulé (avatar animé à l'écran), tout le logiciel sur PC, Raspberry Pi en option
- **Décision :** option 2.
- **Justification :**
  - plus personne dans l'équipe n'a les compétences matériel ;
  - suppression des risques de livraison, de budget et de pannes électroniques ;
  - le temps gagné va au cœur du sujet : interaction (ILMSI) et sécurité (Cyber) ;
  - le traitement reste 100 % local (PC du domicile), l'argument vie privée est conservé.
- **Conséquences :**
  - robot physique hors périmètre ; budget matériel quasi nul ;
  - ambition renforcée côté Cyber (EBIOS RM, authentification et traçabilité des commandes critiques, test d'intrusion) et ILMSI (appli aidant, backend, interface pour seniors) ;
  - portage sur Raspberry Pi possible après la Commission 3 si le temps le permet (durcissement d'un objet connecté par le binôme Cyber).
