# 📌 Projet THE GAME REVIEW

Bienvenue dans le projet **THE GAME REVIEW** ! Ce site est conçu pour offrir aux joueurs une plateforme dédiée à la découverte et au partage de leurs expériences avec d'autres passionnés.

---

## Membre du projet
- Evan FERRON
- Evan GUILLET
- Maxime FUZEAU
- Matias BELLAUD

## 📂 Structure du projet

```
├── .env
├── .env.exemple
├── .gitignore
├── create_local_database.ts
├── DEV.README.md
├── index.ts
├── package-lock.json
├── package.json
├── README.md
├── src
│  ├── base                # Classes de base pour une architecture commune
│  │  ├── AController.ts   # Classe parent des controllers
│  │  ├── AError.ts        # Classe parent des erreurs
│  │  └── ARepository.ts   # Classe parent des repositories
│  ├── config              # Configuration du projet
│  │  └── config.ts
│  ├── database            # Connexion à la base de données et repositories
│  │  ├── database.ts
│  │  └── repositories
│  │    ├── review.ts
│  │    └── user.ts
│  ├── docs                # Documentation
│  ├── modules             # Modules indépendants
│  │  ├── auth             # Gestion de l'authentification
│  │  │  ├── controller.ts
│  │  │  └── routes.ts
│  │  ├── review          # Module Review
│  │  │  ├── controller.ts
│  │  │  └── routes.ts
│  │  └── user            # Module User
│  │    ├── controller.ts
│  │    └── routes.ts
│  ├── routes              # Gestion centralisée des routes
│  │  └── index.ts
│  └── shared              # Code réutilisable
│    ├── error
│    │  └── ApiError.ts    # Gestion des erreurs applicatives
│    ├── index.ts
│    ├── middleware       # Middleware d’authentification et d’erreurs
│    │  ├── auth.ts
│    │  └── error.ts
│    ├── models           # Interfaces et modèles globaux
│    │  └── IModels.ts
│    └── utils            # Utilitaires
│      └── jwt.ts         # Gestion des JWT
├── tree.tree
└── tsconfig.json
```


## 🚀 Installation

### 1️⃣ Prérequis
- Node.js (version recommandée : 18.x ou supérieure)
- npm ou yarn

### 2️⃣ Installation des dépendances
```sh
npm install  # ou yarn install
```

### 3️⃣ Configuration de l'environnement
Copiez le fichier `.env.example` et renommez-le en `.env`. Remplissez les valeurs nécessaires.

### 4️⃣ Démarrer le projet
```sh
npm run dev  # ou yarn dev
```

---

## 🛠 Bonnes pratiques

- **Respectez la structure des dossiers** 📂
- **Utilisez TypeScript** 🟦 pour des types forts et éviter les erreurs
- **Évitez d'écrire la logique métier dans les composants** 🏗️, privilégiez les hooks ou services
- **Utilisez Prettier et ESLint** 🎨 pour garder un code propre et homogène
- **Divisez votre code en composants réutilisables** ⚛️
- **Pensez à mettre à jour la documentation** 📝 lorsque vous modifiez des fonctionnalités
