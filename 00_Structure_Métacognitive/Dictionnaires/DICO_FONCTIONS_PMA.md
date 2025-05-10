---
titre: "Dictionnaire des Fonctions – Projet Mémoire Augmentée (PMA)"
type: dictionnaire_fonctions
date: 2025-05-09
statut: actif
---

## 🔄 Fonction : `UPDATE_MERGE_QUEUE`
- **Nom** : `UPDATE_MERGE_QUEUE`
- **But** : Mettre à jour automatiquement ou manuellement le fichier `MERGE_QUEUE.md` à chaque création ou réception de fichier PMA.
- **Type** : Fonction réflexe de gestion d’intégration
- **Statut** : `wip`
- **Déclenchement** :
  - Automatique : à chaque génération d’un fichier `.md` dans une session SMA
  - Manuel : sur réception explicite d’un fichier utilisateur
- **Paramètres clés** :
  - `Nom du fichier`
  - `Date de création`
  - `Type` (idée, protocole, journal, etc.)
  - `Contexte SMA`
  - `Destination proposée`
  - `Stratégie` (Option A ou B)
  - `Statut` (en attente, intégré, validé)
- **Appuis cognitifs** :
  - `chrono-conscience` : rattachement temporel du fichier
  - `topo-conscience` : rattachement topologique dans le PMA
- **Fichier cible** : `MERGE_QUEUE.md`

---

## 📌 Notes
- Cette fonction est appelée à devenir un **mécanisme central du pilotage mémoire SMA_M1**.
- Elle est conçue pour **favoriser la traçabilité, la planification des fusions, et l’activation de modules**.



---

## 🔄 Fonction : `FUSE_MERGE_QUEUE`
- **Nom** : `FUSE_MERGE_QUEUE`
- **But** : Traiter intelligemment la file `MERGE_QUEUE.md` pour intégrer les fichiers dans leur destination finale selon stratégie définie.
- **Type** : Fonction réflexe d’orchestration mémoire
- **Statut** : `wip`
- **Déclenchement** :
  - Manuel ou déclenché par un agent SMA (ex : Agent_Fusionneur)
- **Paramètres clés** :
  - `Nom du fichier`
  - `Destination`
  - `Stratégie` (Option A / B)
  - `Statut`
- **Appuis cognitifs** :
  - `chrono-conscience` : priorisation par date
  - `topo-conscience` : distribution dans l’arborescence SMA
  - `intention-contextuelle` : adaptation du mode d’intégration au type de contenu
- **Fichier source** : `MERGE_QUEUE.md`

## 📌 Notes
- Fonction miroir de `UPDATE_MERGE_QUEUE`
- Centralise la **décision d’intégration** (fusion directe, regroupement différé, archivage, etc.)
- Vise à limiter la dispersion et à maintenir la **cohérence cognitive** du système

