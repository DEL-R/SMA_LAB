# CONVENTION_BRANCHE.md

## Objectif

Distinguer clairement les usages de :
- Branches Git techniques
- Branches conceptuelles PMA
- Dossiers de classement
- Fichiers `.meta`

---

## 1. Branche Git

Exemples : `main`, `archive`, `dev`, `v0.2`
- Usage : versionner les changements du dépôt, suivre l'évolution du projet dans Git
- Portée : technique

## 2. Branche PMA (conceptuelle)

Exemples : `GENESIS`, `AGENTS`, `PROTOCOLES`, `RITUELS`
- Usage : segmenter les contenus selon leur fonction cognitive
- Portée : organisation mentale et sémantique
- Mise en œuvre : via arborescence de dossiers

## 3. Dossier logique

Exemples :
- `00_GENESIS/` : les fondations
- `10_RITUELS/` : routines déclenchables
- `20_AGENTS/` : description d'agents
- `30_PROTOCOLS/` : fichiers de fonctions cognitives

## 4. Fichier .meta

Exemples : `.meta_01_Noyau_PMA.md`
- Usage : porter les métadonnées d’un fichier principal
- Sert à : lier, documenter, annoter pour agents ou humains

---

## Résumé

- 🛠️ Git = versionnage
- 🧠 PMA = logique cognitive
- 📂 Dossiers = structure visible
- 🧾 .meta = annotation vivante
