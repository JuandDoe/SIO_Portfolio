# 📚 **Dictionnaire de Données - Pikascrape**

## 1. Introduction 🎯
Ce dictionnaire de données décrit la structure des données du projet **[Pikascrape]**, permettant aux développeurs, analystes, et administrateurs de base de données de comprendre la signification, les types et les contraintes des données.

---

## 2. Table des Matières 📑
1. [Introduction](#1-introduction-)
2. [Table des Matières](#2-table-des-matières-)
3. [Structure des Données](#3-structure-des-données-)
   - [Tables](#31-tables-)
   - [Dictionnaire des Colonnes](#32-dictionnaire-des-colonnes-)
4. [Glossaire des termes](#4-glossaire-des-termes-)
5. [Conclusion](#5-conclusion-)

---

## 3. Structure des Données 🗂️

### 3.1. Tables 📋
Voici les tables principales de la base de données, avec une description et leurs responsables.

| **Nom de la Table** | **Description**                                                  | **Responsable** | **Date de Création** |
| ------------------- | ---------------------------------------------------------------- | --------------- | -------------------- |
| **Users**           | Stocke les informations des utilisateurs                         | Admin BDD       | 01/01/2024           |
| **Bookmarks**       | Stocke les requêtes de prix de cartes favorites des utilisateurs | Admin BDD       | 01/01/2024           |

---

### 3.2. Dictionnaire des Colonnes 🛠️

#### **Table : Utilisateurs**

| **Nom de la Colonne** | **Type de Donnée** | **Description**                            | **Contraintes**             |
| --------------------- | ------------------ | ------------------------------------------ | --------------------------- |
| **user_id**           | SERIAL4            | Identifiant unique de l'utilisateur        | PRIMARY KEY, AUTO_INCREMENT |
| **username**          | VARCHAR(255)       | Nom de l'utilisateur                       | NOT NULL                    |
| **email**             | VARCHAR(255)       | Adresse email unique                       | NOT NULL, UNIQUE            |
| **telegram_id**       | VARCHAR(255)       | Identifiant Telegram de l'utilisateur      | NOT NULL                    |
| **password_hash**     | VARCHAR(255)       | Mot de passe chifré de l'utilisateur       | NOT NULL                    |
| **created_at**        | TIMESTAMP          | Date de la création du compte              | NOT NULL                    |
| **updated_at**        | TIMESTAMP          | Date de la derniére modification du compte | NOT NULL                    |

#### **Table : Bookmarks**

| **Nom de la Colonne** | **Type de Donnée** | **Description**                     | **Contraintes**             |
| --------------------- | ------------------ | ----------------------------------- | --------------------------- |
| **bookmark_id**       | SERIAL4            | Identifiant unique du bookmark      | PRIMARY KEY, AUTO_INCREMENT |
| **user_id**           | SERIAL4            | Identifiant unique de l'utilisateur | NOT NULL                    |
| **url**               | VARCHAR(255)       | Url du produit                      | NOT NULL                    |
| **created_at**        | TIMESTAMP          | Date de la création du bookmark     | NOT NULL                    |
| **updated_at**        | TIMESTAMP          | Date de la dernière modification    | NOT NUL                     |

---

## 4. Glossaire des Termes 📖

| **Terme**       | **Définition**                                                              |
| --------------- | --------------------------------------------------------------------------- |
| **Utilisateur** | Personne ayant un compte et accédant au système                             |
| **Telegram**    | Application de messagerie. Permet de rcevoir des notifications              |
| **Bookmarks**   | url enregistré par un utilisateur pour réaliser une requête plus rapidement |

---

## 5. Conclusion 🎯
Ce dictionnaire doit être mis à jour régulièrement pour suivre l'évolution des données et des fonctionnalités du projet. Toute modification doit être documentée pour garantir une cohérence dans la gestion des données.

