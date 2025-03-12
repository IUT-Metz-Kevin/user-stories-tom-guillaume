# 🗂 Example Mapping - Learn@Home

L'Example Mapping permet de structurer la compréhension des User Stories en identifiant les **règles de gestion**, les **exemples concrets** et les **questions en suspens**.

---

## 📌 1. Connexion au site
> **User Story :** En tant qu'utilisateur (élève ou bénévole), je veux me connecter avec mon identifiant et mon mot de passe afin d'accéder à mon espace personnel.

| **Règles** | **Exemples** | **Questions** |
|------------|-------------|--------------|
| L’utilisateur doit saisir un **email et un mot de passe valides** | ✅ Identifiants corrects → Connexion réussie, redirection vers tableau de bord | L’administrateur doit-il aussi passer par cette interface ? |
| Si l’identifiant ou le mot de passe est incorrect, un **message d’erreur clair** doit apparaître | ❌ Mot de passe incorrect 3 fois → Message d’erreur | Le verrouillage du compte doit-il expirer après un certain temps ? |
| Après **5 tentatives échouées**, le compte est **verrouillé temporairement** | ❌ Mot de passe incorrect 5 fois → Compte verrouillé temporairement, email envoyé | Faut-il envoyer une notification par email après une connexion réussie ? |
| Un bouton "Mot de passe oublié" permet de **réinitialiser le mot de passe** via email | ✅ "Mot de passe oublié" → Email de réinitialisation envoyé |  |
| Une option **"Se souvenir de moi"** permet de **rester connecté** | ✅ Session maintenue après fermeture du navigateur |  |

---

## 📌 2. Création de compte
> **User Story :** En tant qu’administrateur, je veux pouvoir créer un compte pour un élève ou un bénévole afin qu’ils puissent accéder à la plateforme.

| **Règles** | **Exemples** | **Questions** |
|------------|-------------|--------------|
| Seul **l’administrateur** peut créer un compte | ✅ Admin crée un compte élève → Email envoyé avec identifiants | Combien de temps le lien d’activation est-il valide ? |
| L’admin doit renseigner **Nom, Email unique, Type de compte (Élève/Bénévole)** | ❌ Email déjà utilisé → Message d’erreur | Un administrateur peut-il supprimer un compte utilisateur ? |
| Un email automatique contenant **un lien d’activation et un mot de passe temporaire** est envoyé | ✅ Lien d’activation cliqué → Demande de création d’un nouveau mot de passe | Un élève peut-il demander la suppression de son compte ? |

---

## 📌 3. Gestion des tâches
> **User Story :** En tant que bénévole, je veux pouvoir attribuer des tâches aux élèves afin de les aider à organiser leur travail scolaire.

| **Règles** | **Exemples** | **Questions** |
|------------|-------------|--------------|
| Un **bénévole** peut assigner des tâches à un élève qu’il suit | ✅ Bénévole crée une tâche → L’élève la voit dans son espace | Peut-on définir une priorité sur les tâches (basse, moyenne, haute) ? |
| Un **élève** ne peut créer que des tâches pour lui-même | ❌ Élève tente de créer une tâche pour un autre élève → Message d’erreur | Un bénévole peut-il modifier une tâche qu’il a créée pour un élève ? |
| Chaque tâche comprend **Titre, Description, Date d’échéance (optionnelle), Statut ("à faire", "en cours", "terminé")** | ✅ Élève marque une tâche comme "terminée" → Mise à jour immédiate | Les tâches terminées doivent-elles être supprimées ou archivées ? |

---

## 📌 4. Chat en temps réel
> **User Story :** En tant qu’élève, je veux pouvoir discuter en temps réel avec mon bénévole afin d’obtenir de l’aide immédiatement.

| **Règles** | **Exemples** | **Questions** |
|------------|-------------|--------------|
| Un élève ne peut **discuter qu’avec son tuteur assigné** | ✅ Élève envoie un message → Bénévole reçoit la notification | Peut-on envoyer des fichiers dans le chat ? |
| Un bénévole peut discuter avec **plusieurs élèves** | ❌ Élève tente d’envoyer un message à un autre élève → Message refusé | L’historique des messages est-il conservé indéfiniment ? |
| L’interface doit afficher **Photo de profil, Indicateur "lu/non lu", Horodatage** | ✅ Bénévole envoie un message → Élève voit "Lu" après l’ouverture | Un élève peut-il supprimer ses messages ? |

---

## 📌 5. Planification des rendez-vous (Calendrier)
> **User Story :** En tant qu’élève, je veux voir mes rendez-vous planifiés avec mon bénévole afin de mieux organiser mon emploi du temps.

| **Règles** | **Exemples** | **Questions** |
|------------|-------------|--------------|
| Un élève peut consulter la **liste de ses rendez-vous** | ✅ Élève ouvre le calendrier → Voit les prochains rendez-vous | Un élève peut-il proposer une date de rendez-vous ? |
| Un bénévole peut **ajouter, modifier, supprimer** un rendez-vous | ✅ Bénévole ajoute un rendez-vous → L’élève reçoit une notification | Peut-on synchroniser le calendrier avec Google Agenda ? |
| Un email de confirmation est envoyé après chaque action | ✅ Bénévole supprime un rendez-vous → L’élève est informé immédiatement | Combien de temps les rendez-vous passés restent-ils visibles ? |

---
