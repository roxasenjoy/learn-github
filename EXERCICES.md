# EXERCICES — Projet fil rouge *NovaCom*
> **Objectif global** : se familiariser avec Git & GitHub à travers la réalisation d’un **site vitrine statique** pour le client fictif **NovaCom**.  
> **Deux temps** : 1) série d’exercices **solo** (12) ; 2) série d’exercices **en équipe de 3** (12).  
> **Important** : ce document **ne donne volontairement aucune commande**. Vous devez choisir et appliquer les bonnes actions Git/GitHub (locales et distantes) en fonction des consignes.

---

## Matériel fourni (à préparer par l’enseignant)
- Un **dépôt modèle** GitHub servant de point de départ : **<INSÉRER_LIEN_DU_DÉPÔT_MODÈLE>**  
  *(Ex. “Use this template” ou “Fork” activé)*
- Contenu minimal du modèle :  
  - `index.html`, `services.html` (brouillon), `contact.html` (brouillon)  
  - `assets/` (images, `styles.css` minimal)  
  - `README.md` (présentation du projet)  
  - `.gitignore` (basique adapté au projet)

> **Rappel** : le travail consiste à **récupérer** ce dépôt, **travailler localement**, **enregistrer** vos changements, **publier** vos mises à jour, puis **collaborer** via branches, PR et reviews.

---

## Règles d’or
- Des **commits petits et cohérents** avec des messages **clairs** (voix impérative).  
- Une **branche par objectif** (fonctionnalité/correction).  
- Avant de fusionner : **mettre à jour** sa branche par rapport à la branche principale.  
- **PR descriptives** (contexte, captures si utile, check-list).  
- Tenir à jour un **journal d’apprentissage** (`journal-apprentissage.md`) : décisions, problèmes, solutions.

---

# PHASE 1 — Exercices **SOLO** (12)
Vous travaillez **seul** sur votre copie du projet (créée à partir du dépôt modèle).

### S01 — Récupération & installation personnelle
**But :** démarrer sur de bonnes bases.  
**Consignes :**
1. Dupliquer le dépôt modèle (**template** ou **fork**) vers **votre compte**.  
2. **Récupérer** le projet en local.  
3. Ajouter dans `README.md` une courte présentation personnelle (prénom, objectif du site).  
4. Préparer `journal-apprentissage.md` et noter ce que vous avez fait/observé.
**Critères de validation :** le dépôt distant est créé sous votre compte, le projet s’ouvre localement, `README.md` + `journal-apprentissage.md` existent.

### S02 — Première amélioration du site
**But :** cycle local → distant (enregistrer / publier).  
**Consignes :**
1. Ajouter un **en-tête** (logo fictif + navigation) sur `index.html`.  
2. Styliser l’en-tête dans `assets/styles.css`.  
3. **Enregistrer** localement des changements cohérents (granularité).  
4. **Publier** sur le dépôt distant.  
**Validation :** en ligne, l’en-tête est visible ; l’historique est propre (1–2 unités de travail cohérentes).

### S03 — Issue → Branche → PR (en solo)
**But :** isoler une fonctionnalité et la proposer via PR.  
**Consignes :**
1. Créer une **issue** “Créer la page Services (v1)”.  
2. Ouvrir une **branche dédiée** liée à cette issue.  
3. Compléter `services.html` avec **3 services** (texte + icône/illustration).  
4. Ouvrir une **PR** vers la branche principale : titre, description, captures (si utile), check-list.  
5. **Fusionner** la PR.  
**Validation :** PR visible, fusion propre, issue liée (fermée automatiquement si possible).

### S04 — Mise à jour depuis le distant (synchro)
**But :** intégrer des changements distants proprement.  
**Consignes :**
1. Modifier `README.md` **depuis l’interface GitHub** (simulateur de mise à jour distante).  
2. **Récupérer** ces changements sur votre poste.  
3. **Rejouer** vos modifications locales au-dessus de l’état distant si nécessaire (historique **linéaire** attendu).  
**Validation :** pas de “merge inhabituel” ; notez la stratégie retenue dans `journal-apprentissage.md`.

### S05 — Page Contact & sélection des changements
**But :** staging sélectif, commits bien ciselés.  
**Consignes :**
1. Créer/compléter `contact.html` (formulaire non-fonctionnel : nom, email, message).  
2. Structurer en **unités de travail** : structure HTML d’un côté, styles de l’autre.  
3. **Enregistrer** en deux étapes distinctes.  
**Validation :** au moins deux unités cohérentes ; messages explicites.

### S06 — Annulation propre (réparation)
**But :** corriger sans casser l’historique.  
**Consignes :**
1. Introduire volontairement un **style problématique** (ex. contraste illisible).  
2. Valider ce changement, constater le problème.  
3. **Annuler** en créant un enregistrement dédié d’annulation.  
4. Justifier dans `journal-apprentissage.md` pourquoi cette approche est préférable en équipe.  
**Validation :** site redevenu lisible ; historique montrant l’aller-retour contrôlé.

### S07 — Lecture de l’historique
**But :** retracer qui a fait quoi/quand.  
**Consignes :**
1. Trouver **l’enregistrement** qui a modifié pour la dernière fois le **slogan** sur la page d’accueil.  
2. En noter l’identifiant abrégé, l’auteur, la date et le “pourquoi” dans `journal-apprentissage.md`.  
**Validation :** entrée claire dans le journal, vérifiable.

### S08 — Marquer une version (v0.1.0)
**But :** jalonner le projet.  
**Consignes :**
1. Définir le périmètre **v0.1.0** (Accueil + Services v1 + Contact v1).  
2. **Marquer** la version et **publier** ce jalon.  
3. Ajouter un **changelog** succinct dans le `README.md`.  
**Validation :** jalon visible en ligne (onglet “Releases” ou équivalent).

### S09 — Nettoyage de l’historique (squash)
**But :** regrouper des WIP trop fragmentés.  
**Consignes :**
1. Sur une branche de refonte du **pied de page**, avancer par petits pas (plusieurs enregistrements).  
2. **Regrouper** ces pas en une **unité finale** claire avant intégration.  
3. Intégrer proprement dans la branche principale.  
**Validation :** historique final lisible (un seul enregistrement fonctionnel pour le pied de page).

### S10 — Performances & assets
**But :** penser au poids et à l’accessibilité.  
**Consignes :**
1. Ajouter/optimiser quelques **images** (poids raisonnable).  
2. Vérifier la présence d’**attributs alternatifs** pertinents.  
3. Structurer `assets/` proprement (images, styles).  
**Validation :** assets optimisés ; structure claire ; notez vos choix dans le journal.

### S11 — Documentation du dépôt
**But :** clarifier les règles de contribution.  
**Consignes :**
1. Créer `CONTRIBUTING.md` (messages, branches, PR, revue).  
2. Ajouter un **modèle d’issue** simple (bug/feature).  
3. Ajouter un **modèle de PR** (contexte, check-list, captures).  
**Validation :** fichiers en place ; PR/Issues utilisent les modèles.

### S12 — Publication statique (option si autorisé)
**But :** mettre en ligne facilement.  
**Consignes :**
1. Activer la **publication statique** du site (branche principale ou dossier dédié).  
2. Vérifier l’**URL publique** du site.  
**Validation :** site accessible ; l’URL est notée dans le `README.md`.

---

# PHASE 2 — Exercices **ÉQUIPE DE 3** (12)
Créez un **nouveau dépôt d’équipe** (ou une organisation) afin de repartir sur un contexte propre **en groupe**. Rôles tournants conseillés :  
- **A** = lead dev (veille à l’historique & releases)  
- **B** = intégration UI/UX  
- **C** = contenu & accessibilité

### G01 — Kickoff d’équipe
**But :** poser le cadre commun.  
**Consignes :**
1. Créer le dépôt d’équipe ; inviter A, B, C.  
2. Écrire `CONTRIBUTING.md` (messages, nommage branches, PR, revue, “mettre à jour avant fusion”).  
3. **Protéger** la branche principale (revue obligatoire, pas de force push).  
**Validation :** règles publiées ; protections actives.

### G02 — Planification (Issues + Board)
**But :** organiser la charge.  
**Consignes :**
1. Créer des **issues** : hero Accueil, Services v2 (cartes), Témoignages, Accessibilité, Performance, Favicon, Contact v2.  
2. Mettre en place un **project board** (To do / In progress / Review / Done).  
3. **Assigner** les issues (A, B, C).  
**Validation :** board actif, issues priorisées et assignées.

### G03 — Branches de fonctionnalité & PR
**But :** standardiser le flux.  
**Consignes :**
1. Chaque membre crée une **branche** pour son issue (`feat/...`).  
2. Réaliser la fonctionnalité ; ouvrir une **PR** descriptive (contexte, captures, check-list).  
**Validation :** 3 PR ouvertes, liées à leurs issues.

### G04 — Reviews croisées
**But :** qualité collective.  
**Consignes :**
1. Chaque PR reçoit au moins **une review** d’un pair.  
2. Les suggestions sont **appliquées** via de nouveaux enregistrements.  
**Validation :** discussions visibles ; amélioration suite aux retours.

### G05 — Mise à jour avant fusion
**But :** historique propre et à jour.  
**Consignes :**
1. **Actualiser** sa branche par rapport à la branche principale **avant** de fusionner.  
2. Choisir un mode d’intégration privilégiant la **lisibilité** (ex. regrouper).  
**Validation :** historique linéaire ; messages clairs.

### G06 — Conflit maîtrisé
**But :** s’entraîner à résoudre un conflit.  
**Consignes :**
1. Provoquer un **conflit** sur une même ligne (ex. slogan Accueil modifié sur deux branches).  
2. **Résoudre** localement ; **documenter** le choix retenu dans la PR.  
**Validation :** PR fusionnée ; commentaire expliquant la résolution.

### G07 — Accessibilité
**But :** améliorer l’UX pour tous.  
**Consignes :**
1. Ajuster **contrastes** et **taille de police**.  
2. Ajouter des **libellés explicites** aux champs de formulaire, ordre de **tabulation** logique, focus visible.  
**Validation :** checklist d’accessibilité renseignée dans la PR.

### G08 — Performance & assets
**But :** livrer plus léger.  
**Consignes :**
1. Réduire le **poids** des images (format/qualité adaptés).  
2. Simplifier/organiser les **styles** ; supprimer le code mort.  
**Validation :** mesures avant/après notées dans la PR (poids total `assets/`).

### G09 — Release 1.0.0
**But :** figer et livrer.  
**Consignes :**
1. Créer une **branche de release**, corriger les détails.  
2. Rédiger des **notes de version** (nouvelles sections, corrections).  
3. **Publier** la **v1.0.0** (jalon/tag).  
**Validation :** release visible ; notes de version claires.

### G10 — Hotfix 1.0.1
**But :** corriger rapidement après release.  
**Consignes :**
1. Identifier un **bug mineur** (ex. lien cassé).  
2. Créer une **branche hotfix**, corriger, ouvrir une PR, fusionner après review.  
3. **Publier** un correctif **1.0.1**.  
**Validation :** tag patch publié ; notes de version mises à jour.

### G11 — Contribution via fork
**But :** simuler un contributeur externe.  
**Consignes :**
1. Un membre **forke** le dépôt d’équipe.  
2. Dans son fork, préparer une petite amélioration (ex. favicon, meta description).  
3. Ouvrir une **PR depuis le fork** vers le dépôt principal ; suivre `CONTRIBUTING`.  
**Validation :** PR depuis fork acceptée et fusionnée.

### G12 — Qualité continue & rétrospective
**But :** automatiser et capitaliser.  
**Consignes :**
1. Mettre en place une **vérification automatique** simple sur les PR (ex. présence des pages clés, linter HTML/CSS, ou script de contrôle minimal).  
2. Organiser une **rétrospective** : ce qui a bien/mal fonctionné, 3 actions d’amélioration, mise à jour de `CONTRIBUTING.md`.  
**Validation :** la vérification empêche la fusion si elle échoue ; `CONTRIBUTING.md` mis à jour.

---

## Modèles utiles (à copier dans votre dépôt)

### Modèle de Pull Request (exemple)
- **Contexte / objectif :** …  
- **Changements principaux :** …  
- **Checklist :**  
  - [ ] Tests manuels réalisés (navigation, liens, responsive)  
  - [ ] Captures d’écran ajoutées si pertinent  
  - [ ] Documentation mise à jour (README/Contrib)  
  - [ ] Branches synchronisées avec la branche principale

### Modèle d’Issue (exemple)
- **Type :** Bug / Amélioration / Nouvelle fonctionnalité  
- **Description :** …  
- **Étapes / Critères d’acceptation :** …  
- **Impacts potentiels :** …  
- **Ressources / Liens :** …

### Check-list de revue (exemple)
- [ ] Le but de la PR est clair et limité  
- [ ] Les changements sont cohérents et compréhensibles  
- [ ] Nommage des fichiers et sections explicite  
- [ ] Accessibilité minimale respectée (titres, alt, labels)  
- [ ] Pas de régression visible sur les pages existantes  
- [ ] PR synchronisée avec la branche principale avant validation

---
## Conseils
- Documentez vos **décisions** (journal) : “pourquoi” > “comment”.  
- **Petites PR** → retours rapides → meilleure qualité.  
- Privilégiez un historique **lisible** : regroupez les WIP avant d’intégrer.  
- Évitez d’embarquer des **fichiers lourds** ou secrets dans le dépôt.  
- Réutilisez vos **modèles** (issue/PR) et mettez-les à jour au fil des retours.
