# Backend VITALIS - API REST

## Responsable : Membre 1 (Back-end Core + Base de données)

## Technologies
- Django 4.2+
- Django REST Framework
- PostgreSQL
- JWT Authentication

## Installation

1. Créer un environnement virtuel :
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou
venv\Scripts\activate  # Windows
```

2. Installer les dépendances :
```bash
pip install -r requirements.txt
```

3. Configurer les variables d'environnement :
```bash
cp .env.example .env
# Éditer .env avec vos configurations
```

4. Créer la base de données :
```bash
python manage.py migrate
```

5. Créer un superutilisateur :
```bash
python manage.py createsuperuser
```

6. Lancer le serveur de développement :
```bash
python manage.py runserver
```

## Structure du projet

```
backend/
├── vitalis_api/          # Configuration Django principale
├── apps/
│   ├── accounts/        # Gestion des utilisateurs (Patient, Médecin, Hôpital, Admin)
│   ├── patients/        # Gestion des patients
│   ├── doctors/         # Gestion des médecins
│   ├── hospitals/       # Gestion des hôpitaux
│   ├── consultations/   # Gestion des consultations
│   ├── messages/        # Messagerie sécurisée
│   └── chatbot/         # Intégration chatbot
├── core/                # Utilitaires communs
├── static/              # Fichiers statiques
├── media/               # Fichiers uploadés
└── manage.py
```

## Endpoints principaux

- `/api/auth/` - Authentification
- `/api/patients/` - Gestion patients
- `/api/doctors/` - Gestion médecins
- `/api/hospitals/` - Gestion hôpitaux
- `/api/consultations/` - Consultations
- `/api/messages/` - Messagerie
- `/api/chatbot/` - Chatbot

## Documentation API

Une fois le serveur lancé, accéder à :
- Swagger UI : http://localhost:8000/api/swagger/
- ReDoc : http://localhost:8000/api/redoc/

