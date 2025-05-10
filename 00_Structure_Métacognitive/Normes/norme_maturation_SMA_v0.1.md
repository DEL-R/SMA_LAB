# Norme de Maturation SMA – v0.1 (révision validée)

## Philosophie de la norme

Cette norme décrit le **cycle de vie complet** d’une idée, d’une fonction ou d’un module dans le SMA (Système Multi-Agent).  
Elle trace une **courbe de transformation organico-numérique**, depuis l’intuition brute jusqu’au bloc verrouillé, en production.

Elle permet :
- De **nommer chaque étape de maturation**
- De **surveiller** et **tracer** le statut des objets
- D’**éviter les pertes cognitives** en encadrant les flottements

---

## Tableau de référence

| Niveau | Nom de l’étape                | Description courte |
|--------|-------------------------------|--------------------|
| 1      | `IDÉE_NUE`                    | Intuition brute, sans structure |
| 2      | `SCRIPT_ACTIF`                | Fonction testable, non intégrée |
| 3      | `MODULE_EN_DEV`              | Fonction structurée, instable |
| 4      | `MODULE_ASSIGNÉ`             | Fonction portée par un agent ou une structure |
| 5      | `MODULE_FONCTIONNEL`         | Fonction en usage stable dans le système |
| 6      | `MODULE_CRITIQUE_VERROUILLÉ` | Élément vital figé, protégé |

---

## Détail par niveau

### 1. `IDÉE_NUE`

- **Définition** : Pensée émergente, intuition non structurée
- **Marquage** : `?? IDÉE_NUE : [contenu]`
- **Surveillance** : Journal `journal_signaux_captés.md`
- **Analogie** : Graine cognitive non germée

---

### 2. `SCRIPT_ACTIF`

- **Définition** : Fonction testée ponctuellement, appelable à la demande, mais sans structure assignée
- **Marquage** : `%% SCRIPT_ACTIF : [fonction]`
- **Surveillance** : `scripts_actifs.md`
- **Analogie** : Script isolé fonctionnel, hors pipeline

---

### 3. `MODULE_EN_DEV`

- **Définition** : Fonction encapsulée avec nom, logique, doc partielle
- **Marquage** : `### MODULE_EN_DEV : [fonction]`
- **Surveillance** : `dev_modules.md`
- **Analogie** : Classe codée en local, non mergée

---

### 4. `MODULE_ASSIGNÉ`

- **Définition** : Fonction portée (agent, protocole, mémoire, fichier)
- **Marquage** : `### MODULE_ASSIGNÉ : [fonction]`, `Porté par : [x]`
- **Surveillance** : Liste des assignations
- **Analogie** : Fonction intégrée dans un service, API ou pipeline

---

### 5. `MODULE_FONCTIONNEL`

- **Définition** : Fonction stable, utilisée en routine
- **Marquage** : `### MODULE_FONCTIONNEL : [fonction]`
- **Surveillance** : Catalogue SMA principal
- **Analogie** : Composant de production actif

---

### 6. `MODULE_CRITIQUE_VERROUILLÉ`

- **Définition** : Élément fondamental figé – verrouillé, versionné, révisable uniquement via RFC ou duplication
- **Marquage** : `### MODULE_CRITIQUE_VERROUILLÉ : [fonction]`
- **Surveillance** : Registre `core_locked.md`
- **Analogie** : Composant système verrouillé, cœur d’architecture

---

## Remarques

- Chaque module, idée ou projet doit **indiquer son niveau** dans son entête `.md` ou `.py`.
- Des outils d’analyse SMA peuvent suivre automatiquement la progression d’un objet dans cette échelle.
- Le niveau de maturation peut être utilisé pour prioriser, reviewer ou fusionner des branches cognitives.

---