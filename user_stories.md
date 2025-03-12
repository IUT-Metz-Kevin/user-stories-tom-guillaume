# 📖 User Stories - Learn@Home

## 📌 1. Connexion au site
**User Story :**  
> En tant qu'utilisateur (élève ou bénévole), je veux me connecter avec mon identifiant et mon mot de passe afin d'accéder à mon espace personnel.

### ✅ Critères d’acceptation :
- [ ] L’utilisateur doit saisir **son email et son mot de passe** dans les champs dédiés.
- [ ] Si l’email ou le mot de passe est incorrect, un **message d’erreur clair** doit s’afficher.
- [ ] Si le mot de passe est incorrect plus de **5 fois consécutivement**, le compte est **temporairement verrouillé**.
- [ ] Un bouton "Mot de passe oublié" redirige vers une **page de réinitialisation**.
- [ ] Une fois connecté, l’utilisateur est redirigé automatiquement vers son **tableau de bord**.
- [ ] Une **option "Se souvenir de moi"** permet de rester connecté.
- [ ] Une déconnexion entraîne la suppression de la session.

---

## 📌 2. Création de compte
**User Story :**  
> En tant qu’administrateur, je veux pouvoir créer un compte pour un élève ou un bénévole afin qu’ils puissent accéder à la plateforme.

### ✅ Critères d’acceptation :
- [ ] Seul **l’administrateur** peut créer un compte via une interface dédiée.
- [ ] L’admin doit fournir les informations suivantes :
  - [ ] **Nom et prénom**
  - [ ] **Email unique**
  - [ ] **Type d’utilisateur (Élève/Bénévole)**
- [ ] Une vérification s’assure que **l’email n’est pas déjà utilisé**.
- [ ] L’utilisateur reçoit un email avec :
  - [ ] Un **lien d’activation** du compte.
  - [ ] Un mot de passe temporaire.
- [ ] L’utilisateur doit **choisir un nouveau mot de passe** à la première connexion.

---

## 📌 3. Gestion des tâches
**User Story :**  
> En tant que bénévole, je veux pouvoir attribuer des tâches aux élèves afin de les aider à organiser leur travail scolaire.

### ✅ Critères d’acceptation :
- [ ] Un **bénévole** peut créer une tâche et l’assigner à un élève qu’il suit.
- [ ] Un **élève** peut créer des tâches **uniquement pour lui-même**.
- [ ] Chaque tâche doit contenir :
  - [ ] **Un titre obligatoire**
  - [ ] **Une description**
  - [ ] **Une date d’échéance facultative**
  - [ ] **Un statut ("à faire", "en cours", "terminé")**
- [ ] L’élève peut **modifier ou marquer une tâche comme terminée**.
- [ ] Les tâches terminées restent visibles dans un **historique**.
- [ ] Les bénévoles ne peuvent **pas modifier une tâche après sa création**, mais peuvent la supprimer.

---

## 📌 4. Chat en temps réel
**User Story :**  
> En tant qu’élève, je veux pouvoir discuter en temps réel avec mon bénévole afin d’obtenir de l’aide immédiatement.

### ✅ Critères d’acceptation :
- [ ] Un élève ne peut discuter **qu’avec son tuteur assigné**.
- [ ] Un bénévole peut discuter **avec plusieurs élèves** qu’il suit.
- [ ] L’interface doit afficher :
  - [ ] **Photo de profil de l’expéditeur**
  - [ ] **Indicateur "lu/non lu"**
  - [ ] **Horodatage des messages**
- [ ] L’utilisateur peut envoyer des **messages texte uniquement** *(fichiers et images en V2)*.
- [ ] L’utilisateur peut voir **son historique de conversation**.
- [ ] Un message ne peut pas être **modifié** après envoi.

---

## 📌 5. Planification des rendez-vous (Calendrier)
**User Story :**  
> En tant qu’élève, je veux voir mes rendez-vous planifiés avec mon bénévole afin de mieux organiser mon emploi du temps.

### ✅ Critères d’acceptation :
- [ ] L’élève voit tous ses **rendez-vous futurs** sur une interface calendrier.
- [ ] Le bénévole peut :
  - [ ] **Ajouter un rendez-vous** pour un élève qu’il suit.
  - [ ] **Modifier un rendez-vous existant**.
  - [ ] **Supprimer un rendez-vous**.
- [ ] Un email de confirmation est envoyé à l’élève à chaque nouvelle réservation.
- [ ] Les événements passés sont archivés et consultables via un **historique**.

---

## 📌 6. Tableau de bord
**User Story :**  
> En tant qu’utilisateur, je veux voir un résumé de mes tâches, messages et rendez-vous dès ma connexion afin d’avoir une vue d’ensemble claire.

### ✅ Critères d’acceptation :
- [ ] Le tableau de bord affiche :
  - [ ] **Les tâches en cours et à venir** (avec statut)
  - [ ] **Les prochains rendez-vous**
  - [ ] **Le nombre de messages non lus**
- [ ] Un clic sur un élément (tâche, rendez-vous, message) **redirige l’utilisateur** vers la section correspondante.
- [ ] Les informations sont mises à jour en **temps réel**.

---

## 📌 7. Réinitialisation de mot de passe
**User Story :**  
> En tant qu’utilisateur, je veux pouvoir réinitialiser mon mot de passe si je l’ai oublié afin de retrouver mon accès à mon compte.

### ✅ Critères d’acceptation :
- [ ] Un bouton "Mot de passe oublié" est disponible sur la page de connexion.
- [ ] L’utilisateur saisit son email et reçoit un **lien de réinitialisation**.
- [ ] Ce lien expire après **24 heures**.
- [ ] Après validation du lien, l’utilisateur doit saisir **un nouveau mot de passe sécurisé**.

---

## 📌 8. Déconnexion sécurisée
**User Story :**  
> En tant qu’utilisateur, je veux pouvoir me déconnecter de mon compte afin de sécuriser mon accès.

### ✅ Critères d’acceptation :
- [ ] Un bouton "Se déconnecter" est accessible depuis toutes les pages.
- [ ] Après déconnexion, l’utilisateur est redirigé vers la **page de connexion**.
- [ ] La session de l’utilisateur est supprimée immédiatement.

---
