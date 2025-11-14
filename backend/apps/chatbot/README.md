# Chatbot - Membre 6

## Tâches principales

1. **Implémentation du chatbot médical**
   - Intégration NLP basique
   - Réponses aux questions courantes sur SIDA, Cancer, Diabète
   - Intégration dans l'API Django

2. **Messagerie sécurisée**
   - Système de messagerie entre patients et médecins
   - Chiffrement des messages

3. **Support technique**
   - Résolution de bugs d'intégration
   - Tests d'intégration entre composants

## Structure à créer

```
chatbot/
├── models.py          # Modèles pour messages et conversations
├── views.py           # Endpoints API pour chatbot et messagerie
├── serializers.py     # Sérialiseurs Django REST
├── services/          # Logique métier chatbot
│   ├── nlp_service.py
│   └── message_service.py
└── utils/             # Utilitaires
```

## Technologies

- Python (Django)
- NLP basique (spaCy ou NLTK)
- ou API externe (Dialogflow, Rasa)

