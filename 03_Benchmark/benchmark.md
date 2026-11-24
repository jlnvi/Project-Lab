# Benchmark — Assistants et robots compagnons

> Project Lab ESIEE-IT · Équipe 1B Cybercore · Sujet 2 : Interaction multimodale sécurisée
> Objectif : analyser l'existant (demande du jury en Commission 1), repérer ce qui manque pour notre cible et justifier notre positionnement.
> Recherche réalisée en novembre 2026. Prix indicatifs, en dollars quand le produit n'est pas vendu en France.

## Solutions étudiées

| Solution | Type | Cible |
|---|---|---|
| **Amazon Alexa (Echo)** | Assistant vocal grand public | Tout public |
| **ElliQ** (Intuition Robotics) | Robot compagnon de table | Seniors isolés |
| **Reachy Mini** (Pollen Robotics, Hugging Face) | Robot de bureau expressif, open source | Développeurs, makers |
| **Eilik** (Energize Lab) | Petit robot de bureau émotionnel | Enfants, adultes (gadget) |
| **Vector** (Digital Dream Labs, ex-Anki) | Petit robot domestique | Grand public |
| **Notre projet** | Assistant compagnon + robot simulé + appli aidant | Seniors isolés et aidants |

## Comparaison

| Critère | Alexa (Echo) | ElliQ | Reachy Mini | Eilik | Vector | **Notre projet** |
|---|---|---|---|---|---|---|
| Pensé pour les seniors | ✗ | ✓ | ✗ | ✗ | ✗ | **✓** |
| Dialogue utile au quotidien | ✓ | ✓ | À programmer | ✗ | Limité, avec abonnement | **✓** |
| Données traitées en local | ✗ (cloud depuis mars 2025) | ✗ (service connecté) | ✓ possible (open source) | ✓ (hors ligne, mais sans dialogue) | ✗ (cloud) | **✓ 100 % local** |
| Incite à sortir, à garder le lien | ✗ | ✓ | ✗ | ✗ | ✗ | **✓** |
| Lien avec les proches | Appels, messages | ✓ (contact des proches) | ✗ | ✗ | ✗ | **✓ appli aidant** |
| Commandes critiques authentifiées et tracées | ✗ | Non documenté | ✗ | ✗ | ✗ | **✓** |
| Modèle économique | Achat + écosystème Amazon | Abonnement (États-Unis) | 299 $ à 449 $ | 139,99 $ | 399,99 $ + abonnement | **Prototype, matériel ≤ 30 €** |

## Ce qu'on retient de chaque solution

**Amazon Alexa (Echo)** — Depuis le 28 mars 2025, Amazon a supprimé l'option « Do Not Send Voice Recordings » : les requêtes vocales des Echo sont envoyées dans le cloud pour être traitées. La tendance des grands assistants va vers plus de cloud, pas moins. → **Notre différence : le traitement 100 % local.**

**ElliQ** — Robot conçu pour aider les seniors à garder le contact avec leurs proches et à rester actifs. Vendu sur abonnement aux États-Unis ; des programmes publics à New York, en Floride et dans le New Jersey le distribuent gratuitement, et l'État de New York a rapporté une forte baisse du sentiment de solitude chez ses utilisateurs. → **Preuve que le besoin est réel et qu'un compagnon proactif peut aider.** Il est distribué aux États-Unis et repose sur un service connecté.

**Reachy Mini** — Robot de bureau open source qui bouge la tête, parle et écoute ; version Lite à 299 $, version sans fil à 449 $. Pollen Robotics et Hugging Face indiquent ne collecter aucune donnée du robot. C'est une plateforme de développement, sans usage d'accompagnement prévu. → **Inspiration pour l'expressivité, et un simulateur existe : piste pour notre robot simulé.**

**Eilik** — Petit robot émotionnel à 139,99 $, entièrement hors ligne (pas de Wi-Fi, pas de caméra, pas de micro connecté au cloud), mais sans commande vocale. → **Montre qu'un compagnon hors ligne attachant est possible, mais sans dialogue il n'aide pas au quotidien.**

**Vector** — Petit robot domestique vendu 399,99 $ plus un abonnement ; les commandes vocales et les fonctions d'IA passent par le cloud de Digital Dream Labs et dépendent de l'abonnement. → **Risque d'un produit dépendant d'un serveur : s'il s'arrête ou devient payant, le robot perd ses fonctions.**

## Notre positionnement

Aucune solution étudiée ne réunit les quatre points suivants :

1. une cible précise : les seniors isolés et leurs aidants ;
2. un vrai dialogue à la voix ;
3. un traitement 100 % local, sans cloud ni abonnement ;
4. des commandes critiques authentifiées et tracées.

**Notre place : l'expressivité d'un compagnon (robot simulé), le dialogue d'un assistant et une IA 100 % locale, pensés pour les seniors isolés et leurs aidants.**

## Sources

- TechCrunch — [Amazon's Echo will send all voice recordings to the cloud starting March 28](https://techcrunch.com/2025/03/15/amazons-echo-will-send-all-voice-recordings-to-the-cloud-starting-march-28) (mars 2025)
- ElliQ — [FAQ officielle](https://elliq.com/pages/faqs) et [page produit](https://elliq.com/pages/holidays)
- Robotics 24/7 — [Intuition Robotics launches ElliQ for subscription in the U.S.](https://www.robotics247.com/article/intuition_robotics_launches_elliq_companion_robot_us_subscription) (mars 2022)
- Entrepreneur — [Seniors are building deep bonds with this friendly AI robot](https://www.entrepreneur.com/business-news/a-new-ai-robot-is-helping-seniors-combat-loneliness/502676) (février 2026)
- Hugging Face — [Reachy Mini, the open-source robot](https://huggingface.co/blog/reachy-mini)
- Engadget — [You can now pre-order Hugging Face's Reachy Mini robots](https://www.engadget.com/ai/you-can-now-pre-order-hugging-faces-reachy-mini-robots-135925714.html)
- Keyi Robot — [Eilik robot buying guide](https://keyirobot.com/en-us/blogs/buying-guide/eilik-robot)
- Robotics 24/7 — [Digital Dream Labs ships upgraded Vector 2.0](https://www.robotics247.com/article/digital_dream_labs_ships_upgraded_vector_2_0_social_robot) (décembre 2022)
- iFixit — [Anki Vector](https://ifixit.com/Device/Anki_Vector)
