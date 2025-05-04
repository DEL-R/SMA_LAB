# 🔁 Interopérabilité agents ↔ mémoire SMA

## 📚 Contexte

Dans un système multi-agents (SMA) localisé, chaque agent doit pouvoir :

- Lire des informations pertinentes dans une mémoire structurée
- Écrire ou mettre à jour certains fichiers
- Savoir où, comment, et dans quel format interagir

La mémoire étant versionnée (via Git) et structurée en fichiers Markdown, cela impose un besoin d’**interopérabilité formelle**.

---

## 🎯 Objectif

> Permettre à tout agent (ou script) d’interagir avec la mémoire SMA de manière fiable, structurée, et traçable.

Cela implique :
- Une **convention de structuration** (emplacement, format, métadonnées)
- Une **interface d’accès lisible et documentée**
- Une **mémoire organisée comme un graphe navigable** (ou arborescence claire)

---

## 🧩 Éléments existants

| Élément | Fonction |
|--------|----------|
| `prompt_templates/` | Spécifie le rôle attendu des agents |
| `journal_accomplissements.md` | Structure datée et reconnaissable pour les logs |
| `README.md` | Expose la structure logique du système |
| `index.md` (futur) | Servira de point d’entrée / table des matières |

---

## 📐 Pistes de normalisation

### 1. Nommage standard
- Fichiers agents : `template_agent_<nom>.md`
- Journaux : toujours prefixés par `## 📅 YYYY-MM-DD`

### 2. Structures internes
- Utilisation de blocs `##`, `###` pour marquer les sections
- Emojis pour signaler les types d’actions (`📘`, `⚠️`, `✅`, `🔁`, etc.)

### 3. Balises internes
- Exemple :  
  `<!-- agent:doc; action:update; target:index.md -->`  
  pour signaler une action agent lisible automatiquement

---

## 🔄 Exemple de cycle agent ↔ mémoire

1. L’agent lit `index.md` et suit les liens vers des fichiers selon son domaine
2. Il effectue une extraction ou une transformation
3. Il crée une proposition de modification sous forme de :
   - commit Git
   - PR simulée
   - fichier tampon en `tmp/agent_doc/`

---

## 🔧 Outils nécessaires (plus tard)

- Script ou agent capable de parser du Markdown
- Convention de commit ou de PR lisible par d’autres agents
- Indexation des fichiers par rôle ou domaine

---

## 🧠 À suivre

- Définir les formats d’échange entre agents (y compris log, messages, mémoire tampon)
- Structurer l’index comme un graphe logique
- Tester un agent "lecture seule" qui interroge la mémoire et résume

---

Dernière mise à jour : 2025-05-05
