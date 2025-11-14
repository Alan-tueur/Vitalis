# Structure du Projet VITALIS

```
Vitalis/
│
├── 📁 backend/                          # Membre 1 - Back-end Core
│   ├── apps/
│   │   ├── accounts/                    # Gestion utilisateurs
│   │   ├── patients/                    # Gestion patients
│   │   ├── doctors/                     # Gestion médecins
│   │   ├── hospitals/                   # Gestion hôpitaux
│   │   ├── consultations/               # Consultations médicales
│   │   ├── messages/                    # Messagerie sécurisée
│   │   └── chatbot/                     # Membre 6 - Chatbot
│   ├── core/                            # Utilitaires communs
│   ├── static/                          # Fichiers statiques
│   ├── media/                           # Fichiers uploadés
│   ├── requirements.txt                 # Dépendances Python
│   ├── .gitignore
│   └── README.md                        # Guide backend
│
├── 📁 frontend_web/                     # Membres 2, 3, 4 - Front-end Web
│   ├── src/
│   │   ├── components/
│   │   │   ├── common/                  # Composants communs
│   │   │   ├── layout/                  # Layout (Header, Sidebar)
│   │   │   └── charts/                  # Composants graphiques
│   │   ├── pages/
│   │   │   ├── patient/                 # Membre 2 - Espace Patient
│   │   │   │   └── README.md
│   │   │   ├── doctor/                  # Membre 3 - Espace Médecin
│   │   │   │   └── README.md
│   │   │   ├── hospital/                # Membre 4 - Espace Hôpital
│   │   │   │   └── README.md
│   │   │   └── admin/                   # Membre 4 - Espace Admin
│   │   │       └── README.md
│   │   ├── services/                   # Services API
│   │   ├── context/                     # State management
│   │   ├── hooks/                       # Custom hooks
│   │   ├── utils/                       # Utilitaires
│   │   └── styles/                      # Styles globaux
│   ├── public/                          # Fichiers publics
│   ├── package.json                     # Dépendances Node.js
│   ├── .gitignore
│   └── README.md                        # Guide frontend web
│
├── 📁 mobile_app/                        # Membre 5 - Application Mobile
│   ├── lib/
│   │   ├── models/                      # Modèles de données
│   │   ├── services/                    # Services API
│   │   ├── providers/                   # State management
│   │   ├── screens/
│   │   │   ├── auth/                    # Authentification
│   │   │   ├── patient/                 # Espace Patient
│   │   │   ├── doctor/                  # Espace Médecin
│   │   │   └── hospital/                # Espace Hôpital
│   │   ├── widgets/
│   │   │   ├── common/                  # Widgets communs
│   │   │   └── charts/                  # Widgets graphiques
│   │   ├── utils/                       # Utilitaires
│   │   └── routes/                      # Routes navigation
│   ├── assets/
│   │   ├── images/                      # Images
│   │   └── icons/                       # Icônes
│   ├── pubspec.yaml                     # Dépendances Flutter
│   └── README.md                        # Guide mobile
│
├── 📁 database/                          # Membre 1 - Base de données
│   └── README.md                        # Scripts SQL et schémas
│
├── 📁 docs/                              # Documentation
│   ├── CDC_VITALIS.tex                  # Cahier des charges
│   ├── CDC_VITALIS.pdf                  # PDF du CDC
│   ├── GUIDE_DEMARRAGE.md               # Guide de démarrage
│   └── REPARTITION_TRAVAIL.md           # Répartition détaillée
│
├── .gitignore                           # Git ignore global
├── README.md                            # README principal
└── STRUCTURE_PROJET.md                  # Ce fichier
```

## Répartition des Espaces de Travail

### 🔧 Backend (Membre 1)
- **Dossier** : `backend/`
- **Fichiers clés** : `apps/`, `core/`, `requirements.txt`
- **Tâche principale** : API REST, Base de données, Authentification

### 👤 Frontend Patient (Membre 2)
- **Dossier** : `frontend_web/src/pages/patient/`
- **Fichiers clés** : Pages React pour l'espace patient
- **Tâche principale** : Interface utilisateur patient

### 👨‍⚕️ Frontend Médecin (Membre 3)
- **Dossier** : `frontend_web/src/pages/doctor/`
- **Fichiers clés** : Pages React pour l'espace médecin
- **Tâche principale** : Interface utilisateur médecin

### 🏥 Frontend Hôpital + Admin (Membre 4)
- **Dossiers** : `frontend_web/src/pages/hospital/` et `admin/`
- **Fichiers clés** : Pages React pour hôpital et admin
- **Tâche principale** : Interfaces hôpital et administrateur

### 📱 Mobile (Membre 5)
- **Dossier** : `mobile_app/`
- **Fichiers clés** : `lib/screens/`, `lib/services/`
- **Tâche principale** : Application mobile Flutter

### 🤖 Chatbot (Membre 6)
- **Dossier** : `backend/apps/chatbot/`
- **Fichiers clés** : Services chatbot, messagerie
- **Tâche principale** : Chatbot et intégrations

## Prochaines Étapes

1. **Chaque membre** doit lire son README.md spécifique
2. **Membre 1** doit setup le backend en premier
3. **Membres 2-5** peuvent setup leurs environnements en parallèle
4. **Communication** : Utiliser les stand-ups quotidiens
5. **Git** : Créer des branches par fonctionnalité

## Ressources

- [Guide de Démarrage](docs/GUIDE_DEMARRAGE.md)
- [Répartition du Travail](docs/REPARTITION_TRAVAIL.md)
- [Cahier des Charges](docs/CDC_VITALIS.pdf)

