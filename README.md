# VITALIS - Plateforme de Suivi Médical

Plateforme numérique de suivi des patients atteints de SIDA, Cancer et Diabète.

## 🏗️ Structure du Projet

```
Vitalis/
├── backend/              # API REST (Django) - Membre 1
├── frontend_web/         # Application Web React - Membres 2, 3, 4
├── mobile_app/           # Application Mobile Flutter - Membre 5
├── database/             # Scripts SQL et schémas - Membre 1
├── docs/                 # Documentation du projet
└── README.md            # Ce fichier
```

## 👥 Équipe et Répartition

### Membre 1 : Back-end Core + Base de données
- **Dossier** : `backend/`
- **Tâches** : API REST, Base de données, Authentification, Déploiement
- **Technologies** : Django, PostgreSQL, JWT

### Membre 2 : Front-end Web - Espace Patient
- **Dossier** : `frontend_web/src/pages/patient/`
- **Tâches** : Interface Patient (Profil, Historique, Paramètres vitaux)
- **Technologies** : React, React Router, Axios

### Membre 3 : Front-end Web - Espace Médecin
- **Dossier** : `frontend_web/src/pages/doctor/`
- **Tâches** : Interface Médecin (Liste patients, Dossiers, Rapports)
- **Technologies** : React, Chart.js, React Query

### Membre 4 : Front-end Web - Espace Hôpital + Admin
- **Dossier** : `frontend_web/src/pages/hospital/` et `frontend_web/src/pages/admin/`
- **Tâches** : Interfaces Hôpital et Administrateur
- **Technologies** : React, Chart.js, React Query

### Membre 5 : Application Mobile Flutter
- **Dossier** : `mobile_app/`
- **Tâches** : Application mobile (tous les espaces)
- **Technologies** : Flutter, Dart, Provider

### Membre 6 : Chatbot + Intégrations
- **Dossiers** : `backend/apps/chatbot/` et intégrations diverses
- **Tâches** : Chatbot, Messagerie, Support technique
- **Technologies** : Python, NLP, Intégration

## 🚀 Démarrage Rapide

### Backend
```bash
cd backend
python -m venv venv
source venv/bin/activate  # ou venv\Scripts\activate sur Windows
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Frontend Web
```bash
cd frontend_web
npm install
npm run dev
```

### Application Mobile
```bash
cd mobile_app
flutter pub get
flutter run
```

## 📋 Technologies Utilisées

- **Backend** : Django, Django REST Framework, PostgreSQL
- **Frontend Web** : React, React Router, Axios, Chart.js
- **Mobile** : Flutter, Dart
- **Base de données** : PostgreSQL
- **Authentification** : JWT
- **Chatbot** : NLP (Python)

## 📝 Documentation

Voir les README.md dans chaque dossier pour plus de détails :
- [Backend README](backend/README.md)
- [Frontend Web README](frontend_web/README.md)
- [Mobile App README](mobile_app/README.md)

## 🔐 Sécurité

- Authentification JWT
- Gestion des rôles (Patient, Médecin, Hôpital, Admin)
- Isolation des données patients
- Chiffrement des données sensibles

## 📞 Contact

Pour toute question, contacter l'équipe de développement.
