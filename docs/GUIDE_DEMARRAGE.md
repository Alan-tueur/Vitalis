# Guide de Démarrage - VITALIS

## Pour chaque membre de l'équipe

### Étape 1 : Cloner le projet
```bash
git clone <url-du-repo>
cd Vitalis
```

### Étape 2 : Configurer votre environnement

#### Membre 1 (Backend)
```bash
cd backend
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou venv\Scripts\activate  # Windows
pip install -r requirements.txt
cp .env.example .env
# Éditer .env avec vos configurations
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

#### Membres 2, 3, 4 (Frontend Web)
```bash
cd frontend_web
npm install
cp .env.example .env
# Éditer .env avec l'URL de l'API (http://localhost:8000/api)
npm run dev
```

#### Membre 5 (Mobile)
```bash
cd mobile_app
flutter pub get
cp .env.example .env
# Éditer .env avec l'URL de l'API
flutter run
```

#### Membre 6 (Chatbot)
```bash
cd backend
# Suivre les mêmes étapes que Membre 1
# Travailler dans backend/apps/chatbot/
```

### Étape 3 : Créer votre branche Git
```bash
git checkout -b feature/votre-nom-espace
# Exemple : feature/steve-patient ou feature/audrey-doctor
```

### Étape 4 : Commencer le développement

Chaque membre travaille dans son espace dédié :
- **Membre 1** : `backend/`
- **Membre 2** : `frontend_web/src/pages/patient/`
- **Membre 3** : `frontend_web/src/pages/doctor/`
- **Membre 4** : `frontend_web/src/pages/hospital/` et `admin/`
- **Membre 5** : `mobile_app/lib/screens/`
- **Membre 6** : `backend/apps/chatbot/`

## Workflow Git

1. **Avant de commencer** : `git pull origin main`
2. **Créer votre branche** : `git checkout -b feature/votre-fonctionnalite`
3. **Faire vos modifications**
4. **Commit régulier** : `git commit -m "Description de vos changements"`
5. **Push** : `git push origin feature/votre-fonctionnalite`
6. **Créer une Pull Request** sur GitHub/GitLab

## Communication

- **Stand-up quotidien** : 10-15 minutes chaque matin
- **Communication** : Discord/Slack pour questions rapides
- **Documentation API** : Membre 1 doit documenter les endpoints au fur et à mesure

## Ressources

- [Documentation Django](https://docs.djangoproject.com/)
- [Documentation React](https://react.dev/)
- [Documentation Flutter](https://flutter.dev/docs)
- [Cahier des Charges](CDC_VITALIS.pdf)

