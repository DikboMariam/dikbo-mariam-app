# 📱 ConversionApp

Une application Android dédiée à la **conversion de devises et d'unités**, développée en Java avec Android Studio.

---

## 📋 Table des matières

- [Aperçu](#aperçu)
- [Fonctionnalités](#fonctionnalités)
- [Architecture](#architecture)
- [Technologies utilisées](#technologies-utilisées)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Structure du projet](#structure-du-projet)
- [API](#api)
- [Contribution](#contribution)
- [Licence](#licence)

---

## 🔍 Aperçu

**ConversionApp** est une application Android permettant d'effectuer des conversions en temps réel. Elle exploite une API REST via **Retrofit** pour récupérer des données à jour, et offre une interface moderne et intuitive grâce à **Material Design**.

---

## ✨ Fonctionnalités

- 🔄 Conversion en temps réel (taux actualisés via API)
- 🌐 Accès Internet pour la récupération des données
- 📐 Interface Material Design moderne
- 🌙 Support du thème sombre (Dark Mode)
- 📱 Compatible avec tous les formats d'écran (Edge-to-Edge)
- 🗂️ Navigation par onglets (ViewPager2)

---

## 🏗️ Architecture

L'application suit une architecture simple orientée **Activity** :

```
MainActivity
    └── Gestion de l'interface principale
         └── Appels réseau via ApiService (Retrofit)
```

---

## 🛠️ Technologies utilisées

| Technologie | Version | Rôle |
|---|---|---|
| **Java** | 1.8 | Langage principal |
| **Android SDK** | API 34 (Android 14) | Plateforme cible |
| **AndroidX AppCompat** | - | Compatibilité descendante |
| **Material Components** | 1.12.0 | UI/UX Material Design |
| **ConstraintLayout** | - | Gestion des mises en page |
| **ViewPager2** | 1.0.0 | Navigation par onglets |
| **Retrofit 2** | 2.9.0 | Client HTTP / appels API |
| **Gson Converter** | 2.9.0 | Désérialisation JSON |
| **Gson** | 2.10.1 | Parsing JSON |
| **JUnit** | - | Tests unitaires |
| **Espresso** | - | Tests instrumentés |

---

## ✅ Prérequis

- **Android Studio** Hedgehog (2023.1.1) ou version supérieure
- **JDK 8** ou supérieur
- **Android SDK** API 23 (Android 6.0 Marshmallow) minimum
- **Connexion Internet** (pour les appels API)
- Un émulateur Android ou un appareil physique

---

## 🚀 Installation

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/DikboMariam/dikbo-mariam-app.git
   cd conversionApp
   ```

2. **Ouvrir dans Android Studio**
   - Lancer Android Studio
   - Cliquer sur **File > Open**
   - Sélectionner le dossier du projet

3. **Synchroniser Gradle**
   - Android Studio détecte automatiquement le fichier `build.gradle.kts`
   - Cliquer sur **Sync Now** si demandé

4. **Lancer l'application**
   - Sélectionner un émulateur ou un appareil connecté
   - Cliquer sur **▶ Run** (ou `Shift + F10`)

---

## 📖 Utilisation

1. Lancer l'application sur votre appareil Android
2. Sélectionner le type de conversion souhaité
3. Entrer la valeur à convertir
4. Consulter le résultat affiché en temps réel

> ⚠️ Une connexion Internet est requise pour obtenir les taux de conversion à jour.

---

## 📂 Structure du projet

```
conversionApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/conversionapp/
│   │   │   │   ├── MainActivity.java       # Activité principale
│   │   │   │   └── ApiService.java         # Interface Retrofit (API)
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   └── activity_main.xml   # Layout principal
│   │   │   │   ├── values/
│   │   │   │   │   ├── strings.xml         # Chaînes de caractères
│   │   │   │   │   ├── colors.xml          # Palette de couleurs
│   │   │   │   │   └── themes.xml          # Thème de l'application
│   │   │   │   └── values-night/           # Thème sombre
│   │   │   └── AndroidManifest.xml         # Configuration de l'app
│   │   ├── test/                           # Tests unitaires
│   │   └── androidTest/                   # Tests instrumentés
│   └── build.gradle.kts                   # Dépendances du module app
├── build.gradle.kts                       # Configuration Gradle racine
├── settings.gradle.kts                    # Paramètres du projet
└── gradle.properties                      # Propriétés Gradle
```

---

## 🌐 API

L'application utilise **Retrofit 2** pour communiquer avec une API REST de conversion.

- **Interface** : `ApiService.java`
- **Client HTTP** : Retrofit 2.9.0
- **Format de données** : JSON (via Gson)
- **Permission requise** : `android.permission.INTERNET`

---

## 🤝 Contribution

Les contributions sont les bienvenues !

1. **Forker** le projet
2. Créer une branche feature :
   ```bash
   git checkout -b feature/ma-fonctionnalite
   ```
3. Committer les modifications :
   ```bash
   git commit -m "feat: ajout de ma fonctionnalité"
   ```
4. Pusher la branche :
   ```bash
   git push origin feature/ma-fonctionnalite
   ```
5. Ouvrir une **Pull Request**

---

## 📄 Licence

Ce projet est sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

<div align="center">

Développé avec ❤️ par **Dikbo Mariam**

</div>
