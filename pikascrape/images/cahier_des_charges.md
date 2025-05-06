# Pikascrape

## 🚀 PROBLÉMATIQUE

Obtenir et exploiter dynamiquement les variations de prix de produits sur un site de vente en ligne. La saisie d'opportunité d'achat-revente est chronophage. **Pikascrape** vise à faciliter cette démarche pour les usagers de [CardMarket](https://www.cardmarket.com/fr/Pokemon).

---

## 📋 CAHIER DES CHARGES

### Fonctionnalités

#### Versions de l'application
- **CLI** : Interface en ligne de commande pour les utilisateurs avancés.
- **GUI** : Interface graphique pour le web et Android, offrant une expérience utilisateur intuitive.

#### Gestion des utilisateurs
- **Administrateur** : 
  - Peut modifier ou supprimer des comptes utilisateurs.
  
- **Utilisateur** :
  - Créer et accéder à son compte.
  - Rechercher des prix de cartes.
  - Enregistrer ses recherches de cartes en favoris.
  - Faire une recherche rapide via ses favoris.

#### Stockage des données
- Les données des comptes utilisateurs et des favoris sont stockées dans une base de données PostgreSQL.

#### Notifications
- Paramétrage de **notifications conditionnelles** basées sur les variations de prix.
- Envoi de notifications sur **Telegram** en cas de variation intéressante.

#### Support et gratitude
- L'utilisateur peut envoyer un **tip en BTC** via le **Lightning Network** pour remercier le développeur.

---

## 🎨 DESIGN DE L'APPLICATION

### Interface Utilisateur
- **CLI** : Simple et épurée avec des commandes claires et des retours utilisateurs interactifs.
- **GUI Web & Android** : Design moderne avec une navigation fluide, incluant des graphiques pour visualiser les tendances de prix.

---

## ⚙️ TECHNIQUES ET TECHNOLOGIES

- **Langages** : Java
- **Frameworks** : JavaFx pour le frontEnd
- **Base de données** : PostgreSQL pour la gestion des utilisateurs et des données de favoris.Graphana pour la visualisation du monitoring
- **API Telegram** : Pour l'envoi de notifications en temps réel.

---

## 🚧 ÉTAPES DE DÉVELOPPEMENT

1. **Analyse des besoins** : Identification des fonctionnalités essentielles.
2. **Conception de l'architecture** : Choix des technologies et design de la base de données.
3. **Développement des fonctionnalités CLI** : Mise en place des commandes de base.
4. **Création de l'interface web** : Développement de la GUI avec les fonctionnalités clés.
5. **Développement de l'application Android** : Adaptation des fonctionnalités pour mobile.
6. **Tests** : Vérification de la robustesse de l'application et correction des bugs.
---

**Préparez-vous à vivre une expérience d'achat optimisée avec Pikascrape !**
