# 🧠 Architecture de la mémoire : centralisée ou distribuée ?

## 📚 Contexte

Le projet SMA repose sur une mémoire versionnée, structurée en fichiers Markdown, hébergée sur GitHub. Cette mémoire doit permettre à plusieurs agents d'accéder, lire, écrire et enrichir le contenu.

Une question fondamentale pour la suite de l’architecture du système est donc :

> Chaque agent doit-il avoir sa propre mémoire dédiée, ou tous doivent-ils utiliser une mémoire centrale partagée ?

---

## ⚖️ Comparaison des approches

### 🗃️ Mémoire centralisée (approche actuelle)

**Principe** : Tous les agents partagent une mémoire commune, structurée de manière cohérente.

**Avantages :**
- Simplicité d’accès
- Vision unifiée de la connaissance
- Suivi global via Git
- Moins de duplication de contenu

**Inconvénients :**
- Risque de conflits d’écriture entre agents
- Besoin d’un système de coordination (protocoles, conventions)
- Moins adapté à des agents très autonomes

---

### 🧩 Mémoire distribuée (une par agent)

**Principe** : Chaque agent a sa propre mémoire (branche Git, fork, ou dépôt séparé).

**Avantages :**
- Spécialisation maximale
- Moins de collisions sur les fichiers
- Agents réellement autonomes (même déconnectés)

**Inconvénients :**
- Synchronisation complexe
- Risque de divergence ou d’incohérences
- Redondance de certaines informations
- Perte de la vision unifiée sans outil de fusion

---

### 🔀 Approche hybride (future piste)

**Principe** : Un tronc commun partagé + une mémoire tampon ou privée temporaire par agent, fusionnée périodiquement.

**Avantage :** équilibre entre coordination et autonomie.

---

## ✅ Position actuelle

Le système utilise **une mémoire centralisée partagée** :
- structurée par rôles (ex : `prompt_templates/`, `50_Travail_IT_Usine/`, etc.)
- versionnée dans un seul dépôt Git
- accessible à tout agent selon des règles définies

Cela reste compatible avec une évolution vers une approche hybride.

---

## 📌 À suivre

- Mettre en place des **conventions d’accès** (espaces par rôle, formats, etc.)
- Réfléchir à un mécanisme de **simulation de mémoire privée par agent** (branches Git ou dépôts temporaires)
- Intégrer cette réflexion à la roadmap du projet

---

Dernière mise à jour : 2025-05-05
