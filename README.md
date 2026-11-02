# ProjetMobileUQAC

Application mobile développée avec Flutter et Firebase dans le cadre d'un cours à l'UQAC (Université du Québec à Chicoutimi).

> permet de parcourir et de commander des snacks et des boissons 

## Fonctionnalités

- Authentification des utilisateurs (inscription / connexion) avec Firebase Auth
- Stockage et lecture des données en temps réel avec Cloud Firestore
- Catalogue de produits par catégories : boissons, sucrés, salés
- Carrousel d'images pour mettre en avant les produits
- Notifications à l'écran (toasts)

## Technologies

| Outil | Rôle |
|-------|------|
| Flutter / Dart | Framework de l'application |
| `firebase_core` | Initialisation de Firebase |
| `firebase_auth` | Authentification |
| `cloud_firestore` | Base de données NoSQL |
| `carousel_slider` | Carrousel d'images |
| `fluttertoast` | Messages de notification |

## Structure du projet

```
├── lib/                 # Code source Dart
├── assets/snacks/       # Images des produits
│   ├── boissons/
│   ├── sucres/
│   └── sales/
├── test/                # Tests
├── android/ ios/ web/   # Plateformes cibles
├── firestore.rules      # Règles de sécurité Firestore
└── firebase.json        # Configuration Firebase
```

## Prérequis

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (Dart ^3.7.2)
- Un éditeur : Android Studio ou VS Code avec les plugins Flutter et Dart
- Un émulateur Android / iOS ou un téléphone connecté
- Un projet [Firebase](https://console.firebase.google.com/) (voir ci-dessous)

## Installation

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/rboulkriat/ProjetMobileUQAC.git
   cd ProjetMobileUQAC
   ```

2. Installer les dépendances :
   ```bash
   flutter pub get
   ```

3. Configurer Firebase:
   ```bash
   dart pub global activate flutterfire_cli
   flutterfire configure
   ```
   Dans la console Firebase, activez Authentication (email / mot de passe)
   et Cloud Firestore.

4. Lancer l'application :
   ```bash
   flutter run
   ```

## Tests

```bash
flutter test
```

## Auteur

Rabab Boulkriat
GitHub : [@rboulkriat](https://github.com/rboulkriat)
