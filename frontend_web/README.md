# Frontend Web VITALIS - React Application

## Responsables
- **Membre 2** : Espace Patient
- **Membre 3** : Espace Médecin  
- **Membre 4** : Espace Hôpital + Administrateur

## Technologies
- React 18.2+
- React Router DOM
- Axios (API calls)
- React Query (State management)
- Chart.js (Visualisations)
- React Hook Form (Formulaires)

## Installation

1. Installer les dépendances :
```bash
npm install
```

2. Configurer les variables d'environnement :
```bash
cp .env.example .env
# Éditer .env avec l'URL de l'API backend
```

3. Lancer le serveur de développement :
```bash
npm run dev
```

L'application sera accessible sur http://localhost:3000

## Structure du projet

```
frontend_web/
├── public/                 # Fichiers publics
├── src/
│   ├── components/         # Composants réutilisables
│   │   ├── common/        # Composants communs (Button, Input, etc.)
│   │   ├── layout/        # Layout components (Header, Sidebar, etc.)
│   │   └── charts/        # Composants de graphiques
│   ├── pages/             # Pages de l'application
│   │   ├── patient/       # Pages Espace Patient (Membre 2)
│   │   ├── doctor/        # Pages Espace Médecin (Membre 3)
│   │   ├── hospital/      # Pages Espace Hôpital (Membre 4)
│   │   └── admin/         # Pages Espace Admin (Membre 4)
│   ├── services/          # Services API
│   │   ├── api.js         # Configuration Axios
│   │   ├── auth.js        # Service authentification
│   │   ├── patients.js    # Service patients
│   │   ├── doctors.js     # Service médecins
│   │   └── hospitals.js   # Service hôpitaux
│   ├── context/           # Context API (State management)
│   ├── hooks/             # Custom hooks
│   ├── utils/             # Utilitaires
│   ├── styles/            # Styles globaux
│   │   └── theme.js       # Charte graphique (bleu/blanc)
│   ├── App.js             # Composant principal
│   └── index.js           # Point d'entrée
└── package.json
```

## Espaces de travail

### Membre 2 - Espace Patient
Travailler dans : `src/pages/patient/`
- Connexion
- Profil
- Historique consultations
- Paramètres vitaux
- Notifications

### Membre 3 - Espace Médecin
Travailler dans : `src/pages/doctor/`
- Connexion
- Liste patients suivis
- Dossier patient
- Rapports médicaux
- Messagerie

### Membre 4 - Espace Hôpital + Admin
Travailler dans : `src/pages/hospital/` et `src/pages/admin/`
- Validation dossiers patients
- Gestion employés
- Tableaux de bord statistiques
- Gestion utilisateurs

## Charte graphique

Couleurs principales :
- Bleu primaire : #1E88E5
- Bleu secondaire : #42A5F5
- Blanc : #FFFFFF
- Gris clair : #F5F5F5
- Texte : #212121

## Communication avec le Backend

L'URL de l'API est définie dans `.env` :
```
REACT_APP_API_URL=http://localhost:8000/api
```

