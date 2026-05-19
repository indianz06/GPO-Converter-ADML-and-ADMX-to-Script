# GPO to Script Converter (v1.6)

Un outil puissant pour convertir les fichiers de modèles d'administration GPO (`.admx`) en scripts de configuration PowerShell, avec une gestion avancée des états et une intégration Cloud optionnelle.

## 🚀 Fonctionnalités clés

* **Conversion flexible :** Analyse des fichiers `.admx` avec prise en charge optionnelle des fichiers de langue `.adml` pour récupérer les descriptions textuelles.
* **Prêt pour le Cloud / Hybride :** Option permettant d'intégre un **Tenant ID** pour lier les scripts à votre environnement Microsoft 365 / Entra ID.
* **Génération structurée :** L'outil sépare automatiquement le résultat en deux catégories distinctes : une pour **activer la politique** et une pour **désactiver la politique**.

## 📁 Structure des fichiers générés

À la fin de l'exécution, l'outil crée un dossier racine nommé **`GPO_Scripts_V16`** parfaitement ordonné :
* Le sous-dossier **`Activer`** regroupe tous les scripts pour **activer la politique**.
* Le sous-dossier **`désactiver`** regroupe tous les scripts pour **désactiver la politique**.

```text
GPO_Scripts_V16/
├── Activer/
│   └── [Scripts_Pour_Activer_La_Politique].ps1
└── désactiver/
    └── [Scripts_Pour_Désactiver_La_Politique].ps1