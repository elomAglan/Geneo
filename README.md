
📘 Documentation du projet – Application Généalogie (Next.js)

1. Introduction
	•	Nom du projet : Application de gestion d’arbre généalogique
	•	Contexte : Développé dans le cadre du test technique SPARK Recruit.
	•	Objectif : Permettre aux utilisateurs de créer, gérer et visualiser un arbre généalogique interactif.

⸻

2. Technologies utilisées
	•	Frontend : Next.js (React, TypeScript)
	•	Backend : API Next.js / Node.js
	•	Base de données : PostgreSQL + Prisma ORM
	•	Auth : NextAuth
	•	UI : TailwindCSS

⸻

3. Fonctionnalités principales

🔑 Authentification
	•	Inscription (nom + email + mot de passe)
	•	Connexion et gestion de session sécurisée
	•	Protection des routes privées

📂 Gestion des projets
	•	Créer un projet (arbre généalogique)
	•	Modifier / Supprimer un projet
	•	Chaque utilisateur ne voit que ses propres projets

🌳 Arbre généalogique
	•	Ajouter / Modifier / Supprimer un membre
	•	Définir les relations parent-enfant (bi-directionnelles)
	•	Interface interactive (drag & drop, zoom, déplacement des nœuds)

💾 Persistance
	•	Données stockées dans PostgreSQL
	•	Prisma utilisé pour les migrations et la gestion des modèles

🎨 UX
	•	Interface responsive
	•	Feedback visuel (toasts, loaders, messages d’erreurs)
	•	Validation côté client et côté serveur

⸻

4. Installation & Lancement

Prérequis
	•	Node.js ≥ 18
	•	PostgreSQL ≥ 14

Étapes
# Cloner le projet
git clone <https://github.com/elomAglan/Geneo.gitrepo>
cd geneo

# Installer les dépendances
npm install

# Configurer les variables d'environnement
cp .env.example .env

# Lancer les migrations Prisma
npx prisma migrate dev

# Démarrer le serveur
npm run dev
