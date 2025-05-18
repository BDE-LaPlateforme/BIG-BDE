# 📚 Tutoriel : Utiliser GitHub Projects pour organiser ton travail

GitHub Projects permet de gérer visuellement ton projet, comme un tableau Kanban. Tu peux y suivre l’avancement de tes tâches avec des **issues**, des colonnes personnalisées (Backlog / Todo / In progress / testing / Done), et collaborer facilement.

---

## 🧱 1. Créer un GitHub Project

1. Va sur ton **repository forké**.
2. Clique sur l’onglet **Projects** (ou "Projets").
3. Clique sur **"New project"**.
4. Choisis **"Kanban"**.
5. Donne-lui un nom, par exemple `Kanban BDE`.
6. Clique sur **"Create project"**.

---

## 🗂️ 2. Ajouter des colonnes

Par défaut, un tableau Kanban contient 3 colonnes, mais tu en créeras **2 de plus** pour structurer encore mieux ton travail : **Backlog** et **Testing**.

Voici la structure recommandée :

- **Backlog**: idées ou tâches à faire plus tard, non encore prioritaires.
- **To do**: tâches prêtes à être commencées, à faire prochainement.
- **In progress**: tâches en cours de développement.
- **Testing**: tâches terminées mais en phase de vérification ou de relecture.
- **Done**: tâches complètement terminées et validées.

➡️ N'oublie pas de déplacer tes issues d’une colonne à l’autre selon l’avancement de ton travail !
> [!NOTE] 
> Lorsque tu ouvres une **pull request (PR)** pour une tâche liée à une issue, tu peux **lier cette PR à l’issue** en ajoutant une phrase comme :
> **Closes #1** (chaque numéro correspond à une PR spécifique, alors vérifiez avant d'aller plus loin)

---

## 📝 3. Créer et lier des issues

Les **issues** sont des tâches ou fonctionnalités à développer.

### Pour en créer une:
1. Va dans l’onglet **Issues** de ton dépôt.
2. Clique sur **"New Issue"**.
3. Donne-lui un titre clair et une description.
4. Clique sur **"Submit new issue"**.

> [!NOTE]
> Utilisez ce patern devant chaque fonctionaliter de votre issues
> ```markdown
> - [ ] Ajouter une image

### Pour l’ajouter au tableau Project:
- Depuis le tableau:
  1. Clique sur **"Add item"** dans une colonne.
  2. Clique sur **"Add an issue"**.
  3. Recherche ou sélectionne l’issue à lier.

---

## 📌 4. Suivre l’avancement

Tu peux déplacer une issue d’une colonne à l’autre en la faisant glisser :

- ⬅️ de "Todo" vers "In progress" pour marquer en cour de développement.
- 🔁 Revenir en arrière n'est pas conseillé.

---

## 👥 5. Assigner des membres

Si tu travailles à plusieurs :

- Dans chaque issue, tu peux cliquer sur **"Assignees"** pour désigner un ou plusieurs responsables.
- Tu peux aussi ajouter des **labels** (par ex. `frontend`, `urgent`, `backend`) pour mieux trier.

---

## 🎯 6. Bonnes pratiques

- ✅ Crée une issue pour **chaque fonctionnalité ou bug**.
- ✅ Mets à jour régulièrement le **Project** (déplace les tâches terminées).
- ✅ Utilise des **checklists** dans les issues pour détailler les sous-tâches.
- ✅ Pense à clore les issues quand elles sont terminées a l'aide de ta PR.

---

## 🧪 Exemple simple

**Issue : Créer la page d’accueil**
```markdown
## Objectif
Développer un espace d’administration complet et sécurisé permettant la gestion efficace des membres, des stocks, des événements et des produits, avec un contrôle précis des rôles et permissions.

## Espace d’administration

- [ ] Créer une interface sécurisée d’authentification pour les admins
- [ ] Implémenter le CRUD pour la gestion des membres (ajout, édition, suppression, listing)
- [ ] Ajouter la gestion des rôles et permissions des membres (admin, staff, etc.)
- [ ] Mettre en place un module de gestion de stocks (goodies, boissons, consommables)
- [ ] Créer un système de gestion des événements (création, modification, archivage)
- [ ] Développer la gestion des produits vendus (type boutique en ligne)
