# EXERCICES — Projet fil rouge *NovaCom*
> **Objectif global** : se familiariser avec Git & GitHub à travers la réalisation d’un **site vitrine statique** pour le client fictif **NovaCom**.  
> **Deux temps** : 1) série d’exercices **solo** (12) ; 2) série d’exercices **en équipe de 2** (8).  
> **IMPORTANT — FORK FIRST :** vous **travaillez toujours sur votre fork** (copie personnelle du dépôt modèle), **cloné en local**. Vous ne modifiez jamais le dépôt modèle d’origine. Toutes vos modifications partent de **votre dépôt local** → *push* → **votre fork GitHub** → *PR* si nécessaire.

---

## Règles d’or
- Des **commits petits et cohérents** avec des messages **clairs** (voix impérative).  
- Une **branche par objectif** (fonctionnalité/correction).  
- Avant de fusionner : **mettre à jour** sa branche par rapport à la branche principale.  
- **PR descriptives** (contexte, captures si utile, check-list).  
- Tenir à jour un **journal d’apprentissage** (`journal-apprentissage.md`) : décisions, problèmes, solutions.

---

# 🟩 SOLO — Bases de Git (découverte locale)
⚠️ Toutes les modifications doivent être faites sur votre fork (copie personnelle du dépôt modèle), cloné en local.

### S01 — Initialiser & préparer son dépôt
- Forker le dépôt modèle sur votre compte GitHub.  
- Cloner votre fork en local.  
- Ajouter prénom et objectif du site dans `README.md`.  
- Créer `journal-apprentissage.md`.  
✅ Résultat : dépôt local fonctionnel, fichiers modifiés visibles sur votre fork GitHub après push.

### S02 — Premier commit structuré
- Ajouter un header basique dans `index.html`.  
- Commit clair : *Ajoute en-tête à la page d’accueil*.  
- Push sur votre fork GitHub.  
✅ Résultat : en ligne, l’en-tête apparaît sur votre repo.

### S03 — Cycle complet (modif → stage → commit → push)
- Modifier `styles.css` pour styliser le header.  
- Vérifier l’état avec `git status`.  
- Ajouter sélectivement au staging.  
✅ Résultat : commit clair, visible sur votre fork.

---

# 🟧 SOLO — Git pratique (features & historique)

### S04 — Issue + branche + PR
- Sur votre fork, créer une issue : *Page Services v1*.  
- Nouvelle branche `feat/services`.  
- Ajouter 3 services dans `services.html`.  
- Ouvrir une PR dans votre fork → fusionner.  
✅ Résultat : issue fermée automatiquement, PR visible dans votre fork.

### S05 — Synchro distante (pull / fetch)
- Modifier `README.md` directement via l’interface GitHub (sur votre fork).  
- Récupérer en local (`git pull`).  
- Noter la stratégie choisie dans le journal.  
✅ Résultat : synchro propre, pas de conflit.

### S06 — Commits sélectifs
- Compléter `contact.html` avec formulaire (nom, email, message).  
- Commit 1 : HTML structure.  
- Commit 2 : CSS styles.  
✅ Résultat : 2 commits séparés, visibles dans l’historique de votre fork.

---

# 🟥 SOLO — Approfondissement Git

### S07 — Explorer l’historique
- Retrouver le commit qui a modifié le slogan d’accueil.  
- Noter auteur, date, hash dans `journal-apprentissage.md`.  
✅ Résultat : info vérifiable.

### S08 — Créer un jalon (tag)
- Définir périmètre `v0.1.0` (Accueil + Services + Contact).  
- Tag `v0.1.0` + push sur votre fork.  
- Ajouter changelog dans `README.md`.  
✅ Résultat : release visible dans l’onglet “Releases” de votre repo GitHub.

### S09 — Corriger proprement
- Introduire un bug visuel (mauvaise couleur).  
- Commit = *Ajoute style illisible*.  
- Corriger avec un commit de revert.  
✅ Résultat : historique montre erreur + correction.

---

# ⬛ SOLO — Consolidation

### S10 — Documentation de contribution
- Créer `CONTRIBUTING.md` avec règles (commits, branches, PR).  
✅ Résultat : fichier présent dans votre fork.

### S11 — Organisation des assets
- Ajouter 1–2 images dans `assets/images/`.  
- Vérifier poids raisonnable + alt.  
✅ Résultat : repo mieux structuré.

### S12 — Publication GitHub Pages
- Activer GitHub Pages sur votre fork.  
- Vérifier que l’URL publique fonctionne.  
✅ Résultat : site en ligne, URL notée dans `README.md`.

---

# 🟩 ÉQUIPE DE 2 — Premiers pas collaboratifs
⚠️ L’équipe crée un dépôt partagé (nouveau repo d’équipe ou organisation).  
Chaque membre clone le dépôt équipe en local, et ne travaille jamais directement sur le repo de l’autre.

### G01 — Dépôt commun
- Créer dépôt d’équipe.  
- Inviter le binôme.  
- Ajouter `CONTRIBUTING.md`.  
✅ Résultat : règles visibles sur repo équipe.

### G02 — Issues & Kanban
- Créer 3 issues (Accueil, Services, Contact).  
- Créer un project board simple (To Do / In progress / Done).  
✅ Résultat : board actif, issues assignées.

---

# 🟧 ÉQUIPE DE 2 — Collaboration active

### G03 — Branches de fonctionnalité
- Chaque étudiant crée une branche `feat/...` à partir du dépôt équipe.  
- Dev → ouvrir PR.  
✅ Résultat : 2 PR ouvertes sur le dépôt équipe.

### G04 — Reviews croisées
- Chaque étudiant review la PR de l’autre.  
- Proposer au moins 1 amélioration et l’appliquer.  
✅ Résultat : PR améliorées puis fusionnées.

---

# 🟥 ÉQUIPE DE 2 — Conflits & synchro

### G05 — Mise à jour avant merge
- Rebaser sa branche sur `main` avant de fusionner.  
✅ Résultat : historique propre.

### G06 — Conflit simulé
- Modifier la même ligne dans `index.html` sur 2 branches.  
- Résoudre en local et documenter la décision dans la PR.  
✅ Résultat : PR fusionnée avec explication.

---

# ⬛ ÉQUIPE DE 2 — Projets réels

### G07 — Release 1.0.0
- Créer une branche release.  
- Corriger détails.  
- Tag `v1.0.0` + notes de version.  
✅ Résultat : release visible sur repo équipe.

### G08 — Hotfix 1.0.1
- Simuler bug (ex. lien cassé).  
- Corriger via branche `hotfix/...`.  
- Tag `v1.0.1`.  
✅ Résultat : patch publié avec changelog.
