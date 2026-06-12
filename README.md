# 🔐 Audit de Conformité ISO 27001 — TechSecure Solutions

> Projet académique réalisé dans le cadre du cursus Master 2 Cybersécurité — École 2600  
> Exercice d'audit de système de management de la sécurité de l'information (SMSI)

---

## 📋 Présentation du projet

Ce dépôt contient le rapport d'audit ISO 27001 réalisé pour **TechSecure Solutions**, une PME fictive de 85 collaborateurs spécialisée dans l'édition de logiciels pour le secteur bancaire.

L'exercice vise à simuler un audit de conformité complet en se plaçant successivement dans la posture de l'**audité** (préparation, organisation des preuves) et de l'**auditeur** (identification des écarts, rédaction des constats, plan d'actions).

---

## 🎯 Objectifs pédagogiques

- Comprendre la logique et le déroulement d'un audit ISO 27001
- Se positionner comme équipe auditée face à un organisme de certification
- Raisonner avec la rigueur d'un auditeur tiers indépendant
- Analyser des preuves de conformité et identifier des écarts réalistes
- Proposer des actions correctives pertinentes et traçables
- Rédiger un livrable professionnel structuré selon les attendus de la norme

---

## 🏢 Contexte du scénario

**Entreprise auditée :** TechSecure Solutions  
**Secteur :** Édition logicielle — clients grands comptes bancaires  
**Effectif :** 85 collaborateurs  
**Enjeu :** La certification ISO 27001 conditionne le renouvellement d'un contrat représentant **30 % du chiffre d'affaires annuel** (Banque Régionale de l'Ouest)

### Périmètre du SMSI

| Inclus | Exclus |
|---|---|
| Datacenter de Lyon | Site de Nantes |
| Équipe développement | Applications clients |
| Équipe support/exploitation | Activité calculateurs embarqués |
| Infrastructure IT interne | |
| Processus de développement, déploiement, maintenance | |
| Gestion des accès environnements clients | |

---

## 📂 Structure du rapport

```
│
├── 1. Présentation du contexte et périmètre
│   ├── Présentation de l'entreprise
│   ├── Justification de la certification
│   ├── Périmètre du SMSI
│   └── Parties prenantes
│
├── 2. Préparation de l'audit côté audité
│   ├── Organisation documentaire (outil GRC Tenacy)
│   ├── Pack audit mis à disposition
│   └── Sensibilisation et préparation des équipes
│
├── 3. Analyse de conformité ISO 27001 (5 mesures Annexe A)
│   ├── A.5.15 — Contrôle d'accès
│   ├── A.8.13 — Sauvegarde des informations
│   ├── A.5.24 — Gestion des incidents de sécurité
│   ├── A.6.3  — Sensibilisation et formation
│   └── A.5.19 — Sécurité dans les relations fournisseurs
│
├── 4. Point de vue auditeur
│   ├── 3 Non-conformités formalisées
│   ├── 2 Observations
│   └── 2 Opportunités d'amélioration
│
├── 5. Plan d'actions correctives
│   └── Fiches NC-01 / NC-02 / NC-03 (action, responsable, délai, preuve)
│
└── 6. Conclusion
    ├── Retours d'expérience
    ├── Limites de l'audit
    └── Recommandations stratégiques
```

---

## 🔍 Mesures ISO 27001 analysées

| Référence | Domaine | Statut |
|---|---|---|
| **A.5.15** | Contrôle d'accès | ⚠️ Non-conformité mineure |
| **A.8.13** | Sauvegarde des informations | ❌ Non-conformité majeure |
| **A.5.24** | Gestion des incidents | ⚠️ Observation |
| **A.6.3** | Sensibilisation et formation | ⚠️ Observation |
| **A.5.19** | Sécurité fournisseurs | ❌ Non-conformité majeure |

---

## 🚨 Synthèse des non-conformités

### NC-01 — Défaut de tests de restauration (A.8.13)
- **Constat :** Aucun test de restauration réalisé depuis 14 mois (dernière entrée : 15/11/2024)
- **Risque :** Incapacité à garantir le RTO en cas de sinistre majeur
- **Action :** Test immédiat sur préproduction + calendrier trimestriel
- **Délai :** 15 jours — *Responsable : Administrateur Systèmes*

### NC-02 — Intégration SaaS non auditée (A.5.19)
- **Constat :** Outil CloudTicket déployé en production sans revue de sécurité ni annexe contractuelle
- **Risque :** Fuite potentielle de données bancaires chez un tiers non audité
- **Action :** Évaluation rétroactive + avenant sécurité
- **Délai :** 2 mois — *Responsable : RSSI / Service Achats*

### NC-03 — Revue des accès non formalisée (A.5.15)
- **Constat :** Absence de procès-verbal signé pour la revue de juin 2025
- **Risque :** Maintien d'accès obsolètes (ex-collaborateurs)
- **Action :** Revue de rattrapage + modèle standardisé de compte-rendu
- **Délai :** 3 semaines — *Responsable : DSI*

---

## 👥 Équipe

| Nom |
|---|
| Sam Levy |
| Alberick Mahoussi |
| Lucas Poignard |
| Ahmed Elabaidi |
| Jibril Mahrouf |
| Idriss Taberkane |
| Theo Pavlovic |
| Romain Grégoire |

---

## 🛠️ Outils et référentiels utilisés

- **Norme de référence :** ISO/IEC 27001:2022 (Annexe A)
- **Méthode d'analyse de risques :** EBIOS Risk Manager
- **Outil GRC simulé :** Tenacy
- **Outil de ticketing :** GLPI
- **Outil de sauvegarde :** Veeam Backup
- **Durée d'audit estimée :** 11 jours/homme (ISO 27006, 85 employés)

---

## 📚 Références

- [ISO/IEC 27001:2022 — Information security management systems](https://www.iso.org/standard/27001)
- [ISO 27006 — Requirements for audit and certification bodies](https://www.iso.org/standard/74054.html)
- [Guide EBIOS Risk Manager — ANSSI](https://www.ssi.gouv.fr/guide/ebios-risk-manager-the-method/)

---

## ⚠️ Avertissement

Ce projet est un **exercice académique**. L'entreprise TechSecure Solutions, les données, les incidents et les preuves mentionnées sont entièrement **fictifs**. Ce rapport ne constitue pas un audit de certification réel.
