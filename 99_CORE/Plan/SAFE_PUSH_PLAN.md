# ✅ SAFE_PUSH_PLAN – PMA_2025-05-09 (Version réelle)

> Export GitHub planifié à partir de l’environnement local PMA  
> Statut : PRÉ-FUSION | PASSE 1 + 2 VALIDÉES | ZONE PUBLIQUE STAGÉE

---

## 🧾 Fichiers candidats à l’export

| Fichier                                 | Cible GitHub                              | Statut      |
|----------------------------------------|-------------------------------------------|-------------|
| `DICO_FONCTIONS_PMA.md`                | `/00_Structure_Métacognitive/Dictionnaires/` | ✅ OK       |
| `INDEX_REFLEXES_PMA.md`                | `/00_Structure_Métacognitive/Reflexes/`   | ✅ OK       |
| `norme_maturation_SMA_v0.1.md`         | `/00_Structure_Métacognitive/Normes/`     | ✅ OK       |
| `README_NORMES_SMA.md`                 | `/00_Structure_Métacognitive/Normes/`     | ✅ OK       |
| `manifest_PMA_v0.1.yaml`               | `/99_CORE/`                                | ⚠️ PROTÉGÉ |
| `MERGE_ACTIVE_Fusion_PMA_2025-05-09.md`| `/99_CORE/`                                | ✅ OK       |
| `scan_initial_Fusion_PMA_2025-05-09.md`| `/99_CORE/`                                | ✅ OK       |
| `PASSED2_ZIP_SCAN_FUSION_PMA.md`       | `/98_Labos/Exports/`                       | ✅ OK       |
| `INTEGRATION_PLAN_PMA_2025-05-09.md`   | `/99_CORE/Plans/`                          | ✅ OK       |
| `prompt_Fusion_PMA_2025-05-09_Part1_PC.md` | `/99_CORE/Prompts/`                      | ✅ OK       |
| `Module_PROMPTCORE.md`                 | `/00_Structure_Métacognitive/Modules/`     | ✅ OK       |
| `Module_LATENTS.md`                    | `/00_Structure_Métacognitive/Modules/`     | ✅ OK       |
| `Agent_Archiviste.md`                  | `/00_Structure_Métacognitive/Agents/`      | ✅ OK       |

---

## 🗃️ Archives ZIP (décompressées, en attente d’intégration)

| Archive                                 | Action                                    |
|-----------------------------------------|-------------------------------------------|
| `PROMPTCORE_GIT_TEMPLATE.zip`           | ➤ à migrer vers `/__staging/docs_ref/`    |
| `atelier_SMA_ancrage_pack.zip`          | ➤ modules à rattacher manuellement        |
| `Contextes_Conversationnels_Annexes.zip`| ➤ à fusionner avec `Contextes_...IA.zip`  |
| `ECHO_NULL__branches_conversationnelles_...` | ➤ à intégrer dans `/30_Routines/ECHO_NULL/` |
| `export_chatgpt_projet.zip`             | ➤ à archiver dans `/99_CORE/Exports_Historiques/` |

---

## 🛑 Fichiers en blocage ou à traiter manuellement

| Fichier                      | Raison                                 | Action recommandée      |
|-----------------------------|----------------------------------------|--------------------------|
| `manifest_PMA_v0.1.yaml`    | Fichier critique système               | ⚠️ Validation manuelle    |
| `fiche_rudy.md`             | Contient nom complet utilisateur       | 🔒 Anonymisation suggérée |
| `Contextes_Conversationnels_IA.zip` | Risque de doublon avec `Annexes` | 🔁 Fusion supervisée      |

---

## 🧠 Instructions SMA post-push

- Générer un `README.md` à la racine avec table des dossiers
- Archiver les `.zip` non fusionnés dans `/98_Labos/Archives/`
- Activer le `PROTO_META_EXTRACT()` si fichiers `.meta` doivent être indexés
- Laisser les fichiers en staging **non visibles publiquement par défaut**

