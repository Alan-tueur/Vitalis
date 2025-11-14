# Répartition du Travail - Phase Production MVP

## Vue d'ensemble

| Membre | Responsabilité | Dossier Principal | Technologies |
|--------|---------------|-------------------|--------------|
| **Membre 1** | Back-end + Base de données | `backend/` | Django, PostgreSQL, JWT |
| **Membre 2** | Front-end Patient | `frontend_web/src/pages/patient/` | React, Axios |
| **Membre 3** | Front-end Médecin | `frontend_web/src/pages/doctor/` | React, Chart.js |
| **Membre 4** | Front-end Hôpital + Admin | `frontend_web/src/pages/hospital/` et `admin/` | React, Chart.js |
| **Membre 5** | Application Mobile | `mobile_app/` | Flutter, Dart |
| **Membre 6** | Chatbot + Intégrations | `backend/apps/chatbot/` | Python, NLP |

## Détails par Membre

### Membre 1 - Back-end Core
**Priorités MVP :**
1. ✅ Setup Django + PostgreSQL
2. ✅ Modèles de base (User, Patient, Doctor, Hospital)
3. ✅ Authentification JWT basique
4. ✅ Endpoints API essentiels :
   - `/api/auth/login/`
   - `/api/auth/register/`
   - `/api/patients/` (CRUD)
   - `/api/doctors/` (CRUD)
   - `/api/hospitals/` (CRUD)
   - `/api/consultations/`
5. ✅ Déploiement basique

**Livrables :**
- API REST fonctionnelle
- Documentation Swagger des endpoints
- Base de données opérationnelle

---

### Membre 2 - Front-end Patient
**Priorités MVP :**
1. ✅ Setup React + Routing
2. ✅ Page de connexion
3. ✅ Page profil patient
4. ✅ Historique consultations
5. ✅ Paramètres vitaux (affichage)

**Livrables :**
- Application React Patient fonctionnelle
- Intégration avec API backend
- Design responsive (bleu/blanc)

---

### Membre 3 - Front-end Médecin
**Priorités MVP :**
1. ✅ Setup React + Routing
2. ✅ Page de connexion
3. ✅ Liste des patients suivis
4. ✅ Dossier patient détaillé
5. ✅ Visualisations de données (graphiques)

**Livrables :**
- Application React Médecin fonctionnelle
- Graphiques de santé (Chart.js)
- Intégration avec API backend

---

### Membre 4 - Front-end Hôpital + Admin
**Priorités MVP :**
1. ✅ Setup React + Routing
2. ✅ Page de connexion Hôpital
3. ✅ Validation de dossiers patients
4. ✅ Page de connexion Admin
5. ✅ Tableaux de bord statistiques

**Livrables :**
- Application React Hôpital fonctionnelle
- Application React Admin fonctionnelle
- Tableaux de bord avec statistiques

---

### Membre 5 - Application Mobile
**Priorités MVP :**
1. ✅ Setup Flutter
2. ✅ Authentification mobile
3. ✅ Espace Patient mobile (minimum)
4. ✅ Synchronisation avec API
5. ✅ Notifications locales

**Livrables :**
- Application Flutter fonctionnelle (Android minimum)
- Intégration avec API backend
- Design mobile (bleu/blanc)

---

### Membre 6 - Chatbot + Intégrations
**Priorités MVP :**
1. ✅ Setup chatbot basique (FAQ simple)
2. ✅ Intégration chatbot dans API
3. ✅ Messagerie basique
4. ✅ Tests d'intégration
5. ✅ Documentation technique minimale

**Livrables :**
- Chatbot fonctionnel
- Messagerie opérationnelle
- Documentation README

---

## Timeline MVP (5 semaines)

### Semaine 1 : Setup
- **Membre 1** : Backend setup, base de données, authentification
- **Membres 2-5** : Setup projets front-end/mobile
- **Membre 6** : Recherche solution chatbot

### Semaine 2-3 : Développement
- **Membre 1** : Endpoints API complets
- **Membres 2-4** : Développement interfaces web
- **Membre 5** : Développement app mobile
- **Membre 6** : Développement chatbot

### Semaine 4 : Intégration
- Tous : Intégration des composants
- **Membre 1** : Optimisation, déploiement
- **Membre 6** : Tests d'intégration

### Semaine 5 : Finalisation
- Tous : Corrections bugs
- **Membre 6** : Documentation
- Tests finaux et déploiement

---

## Points de synchronisation

### Daily Stand-up (10-15 min)
- Qu'est-ce que j'ai fait hier ?
- Qu'est-ce que je fais aujourd'hui ?
- Y a-t-il des blocages ?

### Communication API
- **Membre 1** doit documenter les endpoints au fur et à mesure
- Utiliser Swagger/Postman pour partager l'API

### Design System
- Couleurs : Bleu #1E88E5, Blanc #FFFFFF
- Composants communs dans `frontend_web/src/components/common/`

### Git Workflow
- Branche par fonctionnalité : `feature/nom-membre-fonctionnalite`
- Commit régulier avec messages clairs
- Pull Request avant merge dans main

---

## Ressources partagées

- [Cahier des Charges](CDC_VITALIS.pdf)
- [Guide de Démarrage](GUIDE_DEMARRAGE.md)
- Documentation API : http://localhost:8000/api/swagger/ (une fois backend lancé)

