# Planning prévisionnel — Équipe 1B Cybercore

> Project Lab ESIEE-IT · Sujet 2 : Interaction multimodale sécurisée
> Jalons calés sur le calendrier officiel du Project Lab (équipe 1B).

## Diagramme de Gantt

```mermaid
gantt
    title Projet Cybercore 1B — 2026-2027
    dateFormat YYYY-MM-DD
    axisFormat %d/%m

    section Jalons
    Commission 1 (projet validé)          :milestone, c1, 2026-10-21, 0d
    Commission 2 (note de cadrage)        :milestone, c2, 2026-11-27, 0d
    CP2 Conception                        :milestone, cp2, 2026-11-30, 0d
    Commission 3 (conception validée)     :milestone, c3, 2027-02-05, 0d
    CP3 Développement                     :milestone, cp3, 2027-02-08, 0d
    Commission 4 (développement validé)   :milestone, c4, 2027-04-09, 0d
    Commission 5 (soutenance blanche)     :milestone, c5, 2027-04-23, 0d
    Soutenance finale                     :milestone, sf, 2027-04-27, 0d

    section Cadrage
    Périmètre, organisation, risques      :done, cad, 2026-10-01, 2026-11-27

    section Conception
    Comparatif des modèles d'IA sur PC    :conc1, 2026-11-30, 2027-01-08
    Architecture et maquettes de l'appli  :conc2, 2026-12-07, 2027-01-22
    Analyse de risques EBIOS RM           :conc3, 2026-12-07, 2027-02-05

    section Réalisation
    Chaîne vocale complète                :real1, 2027-01-11, 2027-03-05
    Robot simulé (avatar)                 :real2, 2027-02-08, 2027-03-12
    Appli aidant et backend               :real3, 2027-02-08, 2027-03-19
    Authentification et journal           :real4, 2027-02-15, 2027-03-19

    section Sécurisation et tests
    Test d'intrusion                      :test1, 2027-03-15, 2027-04-02
    Tests avec les utilisateurs           :test2, 2027-03-22, 2027-04-09

    section Soutenance
    Démo et dossier final                 :sout, 2027-04-09, 2027-04-27

    section Option
    Portage sur Raspberry Pi durci        :opt, 2027-02-08, 2027-04-02
```

## Jalons et livrables

| Date | Jalon | Livrable | Heures PL |
|---|---|---|---|
| 21/10/2026 | Commission 1 | Projet et axe validés ✓ | — |
| 27/11/2026 | Commission 2 | Note de cadrage (deck + ce dépôt de preuves) | ≈ 13 h |
| 30/11/2026 | CP2 Conception (9h-10h, salle 3.40) | Point d'avancement | — |
| 05/02/2027 | Commission 3 | Dossier de conception, dialogue validé sur PC | ≈ 21 h |
| 08/02/2027 | CP3 Développement (9h-10h, salle 3.40) | Point d'avancement | — |
| 09/04/2027 | Commission 4 | Assistant, appli et sécurité testés | ≈ 46 h |
| 23/04/2027 | Commission 5 | Soutenance blanche, démo | ≈ 2 h |
| 27/04/2027 | Soutenance finale | Démo et dossier final | ≈ 2 h |

Total : 84 h de séances Project Lab, auxquelles s'ajoute le travail à distance pendant les périodes en entreprise. Visios de suivi en semaines 46, 1 et 11.

## Dépendances

- Comparatif des modèles d'IA → chaîne vocale complète → robot simulé → tests utilisateurs.
- Analyse de risques EBIOS RM → architecture → authentification et journal → test d'intrusion.
- Maquettes de l'appli → appli aidant → tests avec les aidants.
- Option Raspberry Pi : seulement si la chaîne vocale est validée sur PC à la Commission 3.

## Points critiques

- **Latence de l'IA locale** : mesurée dès la phase de conception (critère : moins de 5 s).
- **Intégration voix + avatar + appli** : prévoir de la marge avant la Commission 4.
- **Périodes en entreprise** : avancer à distance, suivi par commits et Kanban.
