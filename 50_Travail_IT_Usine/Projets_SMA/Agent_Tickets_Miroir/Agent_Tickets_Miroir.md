# Fiche projet : Agent_Tickets_Miroir

## Objectif
Concevoir un **agent personnel local, passif et discret**, destiné à assister l'utilisateur dans la **gestion quotidienne et hebdomadaire de ses tickets KACE**. L’agent ne remplace aucune tâche métier critique mais **soutient activement la rigueur administrative** (relances, journalisation, suivi) en arrière-plan.

## Contexte
- L’utilisateur est technicien support confirmé, très compétent techniquement mais moins rigoureux dans la tenue administrative des tickets.
- Environnement professionnel structuré avec **KACE** pour la gestion des tickets, **protocoles internes**, **workflows**, **procédures**, et **fichier RACI**.
- L’utilisateur ne souhaite pas une mise en œuvre officielle ni visible, mais **un système local, autonome, privé**, ne traitant que ses propres tickets (entre 10 et 17 en moyenne).
- L’environnement professionnel autorise l’usage de **Microsoft Copilot dans Edge**, qui peut être utilisé comme outil de synthèse intermédiaire pour les tickets.

## Philosophie SMA
- L’agent est **passif** : il **n’agit jamais seul** et **n’interagit pas directement** avec les systèmes de l’entreprise (KACE, utilisateurs, etc.).
- Il **accompagne** l’utilisateur pendant sa **revue hebdomadaire (ou quotidienne) des tickets** en lui suggérant des actions, messages, ou priorisations.
- L’agent **s’ancre dans des comportements existants** : ex. l’ouverture manuelle des tickets dans un navigateur.
- Il reste **strictement local**, non partagé, non exposé.

## Fonctions principales (MVP)
1. **Capture des données**
   - Récupération manuelle (copier-coller ou capture automatique) des tickets consultés.
   - Extraction de données essentielles : ID, titre, date dernière action, statut, auteur, résumé.

2. **Analyse & règles simples**
   - Délai depuis la dernière action : relance suggérée au-delà d’un seuil (ex. 3 jours).
   - Statut + type de ticket = suggestion de clôture ou action selon le fichier RACI.

3. **Génération d’un rapport personnel**
   - Liste des tickets à relancer, à clôturer, à surveiller.
   - Propositions de messages prérédigés pour relance ou clôture.
   - Format : Markdown, HTML ou CSV selon préférence.

4. **Journalisation personnelle (facultatif)**
   - Création d’un journal local par ticket (actions notées, dates, relances, réponses).
   - Objectif : mémoire augmentée locale, rigueur, archivage personnel.

## Intégration de Copilot comme point d’entrée
- Pendant la revue hebdomadaire, l’utilisateur copie le contenu du ticket dans **Copilot (Edge)**.
- Un **prompt prédéfini** permet d’obtenir un résumé structuré : titre, ID, type, résumé, dernières actions, statut.
- Ce résumé est **copié manuellement dans un fichier local** pour être lu par l’agent.
- Ce mécanisme sert de **passerelle contrôlée** entre environnement pro et agent local.

## Contraintes et sécurité
- **Strictement local**, aucun accès réseau requis.
- **Pas de connexion directe à KACE**.
- **Aucune donnée sensible extraite automatiquement**.
- L’agent ne fait que proposer, **l’utilisateur garde 100 % du contrôle**.
- L’usage de Copilot reste **manipulé uniquement par l’utilisateur**, sans automatisme ni extraction massive.

## Ressources disponibles
- **Fichier RACI**
- **Protocoles de traitement** par type de ticket
- **Modèles de messages** utilisés en interne
- **Workflows** définis par l’équipe
- **Copilot intégré à Edge**, accessible avec prompts manuels

## Possibilités futures
- Extension vers la gestion des tickets de Baptiste ou du responsable (si validé).
- Intégration OCR ou scraping léger si autorisé.
- Classification automatique des tickets par thème, urgence ou criticité.
- Interface locale (TUI ou simple frontend HTML) pour gérer les revues.

## Statut
**Projet personnel en cours de conception. Pas en production. Strictement personnel.**

## Prochaine étape possible
- Définir l’**architecture technique minimale** : arborescence, langage (Python), format des fichiers, boucle utilisateur.
- Décrire les **entrées types** (fichiers texte ou captures).
- Commencer le **prototype de rapport hebdomadaire**.
- Rédiger les **prompts types pour Copilot**.
