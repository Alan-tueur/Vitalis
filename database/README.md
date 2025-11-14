# Base de données VITALIS

## Responsable : Membre 1 (Back-end Core)

## Technologies
- PostgreSQL (recommandé)
- ou MongoDB (alternative)

## Scripts SQL

Ce dossier contiendra :
- Scripts de création de la base de données
- Migrations
- Scripts de seed (données de test)
- Schémas de base de données

## Structure de la base de données

### Tables principales :
- `users` - Utilisateurs de base (Patient, Médecin, Hôpital, Admin)
- `patients` - Informations spécifiques aux patients
- `doctors` - Informations spécifiques aux médecins
- `hospitals` - Informations des hôpitaux
- `medical_records` - Dossiers médicaux
- `consultations` - Consultations médicales
- `messages` - Messagerie sécurisée
- `notifications` - Notifications système

## Commandes utiles

### PostgreSQL
```bash
# Créer la base de données
createdb vitalis_db

# Se connecter
psql -U postgres -d vitalis_db

# Exécuter un script
psql -U postgres -d vitalis_db -f script.sql
```

