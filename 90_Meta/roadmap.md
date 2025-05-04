# 🧭 Roadmap SMA – 2025

Cette feuille de route structure l’avancement du projet SMA en plusieurs phases. Elle est évolutive et reflète l’état d’avancement réel du système de mémoire centralisée, des agents spécialisés, et de l’infrastructure d’accueil.

---

## ✅ Phase 1 : Structuration & socle technique (mai 2025)

🎯 Objectif : Finaliser une mémoire exploitable, versionnée, et extensible.

| Étape | Objectif | Détails | Statut |
|-------|----------|---------|--------|
| 1.1 | Ajouter un `LICENSE` au dépôt | Probablement MIT ou CC-BY selon usage | ⏳ |
| 1.2 | Étoffer `50_Travail_IT_Usine/` | Procédures récurrentes, modèles de tickets, sécurité | ⏳ |
| 1.3 | Initier l'inventaire `60_HOMELAB/` | Machines Proxmox, VMs, réseau, backups | ⏳ |
| 1.4 | Créer une navigation claire dans `index.md` | Liens internes, structure explicite | ⏳ |
| 1.5 | Brancher GitHub Actions ou un script de sauvegarde | Commit automatique, zip, backup | ⏳ |
| 1.6 | Passer à SSH pour Git (sécurité) | Création de clé, ajout à GitHub | ⏳ |

---

## 🧠 Phase 2 : Premiers agents et prompts (juin 2025)

🎯 Objectif : Activer des agents spécialisés avec mémoire partagée.

| Étape | Objectif | Détails | Statut |
|-------|----------|---------|--------|
| 2.1 | Finaliser les 3 prompts d'agents (`DOC`, `TICKETS`, `SECURITE`) | Rôles, limites, formats | ⚠️ mis en pause |
| 2.2 | Créer un système d'appels à la mémoire (simulé ou réel) | Syntaxe, conventions, champs standardisés | ⏳ |
| 2.3 | Commencer un premier test local avec un LLM simple | Ex : Mistral 7B, TinyLlama via Ollama | ⏳ |
| 2.4 | Documenter les flux agent ↔ mémoire | en `.md` ou schéma | ⏳ |

---

## 🧩 Phase 3 : Localisation & autonomie (été/automne 2025)

🎯 Objectif : SMA fonctionnel localement, interagissant avec mémoire.

| Étape | Objectif | Détails | Statut |
|-------|----------|---------|--------|
| 3.1 | Hébergement de LLM local dans Proxmox | Conteneur ou VM dédiée | ⏳ |
| 3.2 | Création de l'interface agent ↔ mémoire (API, parser md, etc.) | Prototype de dialogue contextuel | ⏳ |
| 3.3 | Test multi-agents avec partage mémoire centralisée | Coordination via fichiers, queues ou autre | ⏳ |

---

Dernière mise à jour : 2025-05-05
