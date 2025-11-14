# Application Mobile VITALIS - Flutter

## Responsable : Membre 5 (Application Mobile Flutter)

## Technologies
- Flutter 3.10+
- Dart 3.0+
- Provider ou Bloc (State management)
- HTTP (API calls)
- Shared Preferences (Stockage local)

## Installation

1. Installer Flutter : https://flutter.dev/docs/get-started/install

2. Vérifier l'installation :
```bash
flutter doctor
```

3. Installer les dépendances :
```bash
flutter pub get
```

4. Configurer les variables d'environnement :
```bash
cp .env.example .env
# Éditer .env avec l'URL de l'API backend
```

5. Lancer l'application :
```bash
flutter run
```

## Structure du projet

```
mobile_app/
├── lib/
│   ├── main.dart                    # Point d'entrée
│   ├── models/                      # Modèles de données
│   │   ├── patient.dart
│   │   ├── doctor.dart
│   │   ├── hospital.dart
│   │   └── consultation.dart
│   ├── services/                    # Services API
│   │   ├── api_service.dart
│   │   ├── auth_service.dart
│   │   ├── patient_service.dart
│   │   └── doctor_service.dart
│   ├── providers/                   # State management (Provider)
│   │   ├── auth_provider.dart
│   │   └── patient_provider.dart
│   ├── screens/                     # Écrans de l'application
│   │   ├── auth/                   # Authentification
│   │   ├── patient/                # Espace Patient
│   │   ├── doctor/                 # Espace Médecin
│   │   └── hospital/               # Espace Hôpital
│   ├── widgets/                    # Widgets réutilisables
│   │   ├── common/
│   │   └── charts/
│   ├── utils/                      # Utilitaires
│   │   ├── constants.dart            # Constantes (couleurs, etc.)
│   │   └── theme.dart               # Thème (bleu/blanc)
│   └── routes/                     # Routes de navigation
├── android/                        # Configuration Android
├── ios/                            # Configuration iOS
└── pubspec.yaml                    # Dépendances
```

## Espaces à développer

- **Espace Patient** : Profil, Historique, Paramètres vitaux, Notifications
- **Espace Médecin** : Liste patients, Dossier patient, Rapports
- **Espace Hôpital** : Validation dossiers, Gestion employés

## Charte graphique

Couleurs principales (définies dans `lib/utils/constants.dart`) :
- Bleu primaire : Color(0xFF1E88E5)
- Bleu secondaire : Color(0xFF42A5F5)
- Blanc : Colors.white
- Gris clair : Color(0xFFF5F5F5)

## Communication avec le Backend

L'URL de l'API est définie dans `.env` et chargée via `flutter_dotenv`.

