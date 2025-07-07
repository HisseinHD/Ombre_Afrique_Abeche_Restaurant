# 🍽️ Ombre Afrique d’Abéché - Système de Gestion de Restaurant

Bienvenue dans le dépôt officiel du projet **Ombre_Afrique_Abeche_Restaurant**, une solution complète de gestion pour un restaurant traditionnel basé à Abéché, Tchad.  
Ce projet s'appuie sur une base de données relationnelle MariaDB et propose une structure claire pour gérer les **employés**, **commandes**, **factures**, **plats**, **stocks**, et **réservations**.

![Capture d’écran du 2025-07-07 11-20-36](https://github.com/user-attachments/assets/52bbd738-1d46-4915-8360-b2a2616112b8)![Capture d’écran du 2025-07-07 11-20-45](https://github.com/user-attachments/assets/a27792fb-0ed8-4dc0-83fa-a7ebeb64bb45)![Capture d’écran du 2025-07-07 11-20-55](https://github.com/user-attachments/assets/a8f06a2e-bd49-48c0-9c85-74aadfb9ecc1)

---

## 📊 Objectif du projet

Ce projet vise à :

- Digitaliser les processus internes du restaurant (prise de commande, gestion des stocks, facturation)
- Suivre les performances (ventes, paiements, réservations)
- Améliorer la gestion des employés et des fournisseurs
- Proposer une base solide pour des extensions futures (application mobile, dashboard admin, etc.)

---
## 🧠 Approche de conception MERISE
##### En tant que concepteur.trice de bases de données, les actions réalisées sont les suivantes :

##### 🔍 Analyse fonctionnelle
###### Étude du fonctionnement du restaurant à partir de la documentation fournie.

###### Identification des processus clés : gestion des employés, des plats, des commandes, des paiements, des stocks et des réservations.

## 🧩 Identification des entités et relations
#### Entités principales : Employé, Plat, Commande, Facture, Ingrédient, Fournisseur, Réservation

#### Relations :

Un employé peut enregistrer plusieurs commandes.

Une commande donne lieu à une facture.

Un plat est composé de plusieurs ingrédients.

Un ingrédient peut provenir de plusieurs fournisseurs.
## 🧠 Modélisation de la base de données

### 1.Dicitionnaire de données

![Capture d’écran du 2025-07-07 12-11-13](https://github.com/user-attachments/assets/55d6aab4-9fe4-4730-83a6-5a79ec141d60)

![Capture d’écran du 2025-07-07 12-11-28](https://github.com/user-attachments/assets/c62b93c4-db4d-401e-9f19-09ddae83b462)

### 2. 🧩 MCD – Modèle Conceptuel de Données

![Capture d’écran du 2025-07-07 12-11-56](https://github.com/user-attachments/assets/5da63729-be0e-4db2-93f2-570974e635a1)

### 3. 🧩 MLD – Modèle Logique de Données

![Capture d’écran du 2025-07-07 12-11-42](https://github.com/user-attachments/assets/1096271f-2998-4e30-a2c6-2720aeeb1ec4)

### 4. 🧩 MPD – Modèle Physique de Données (Script SQL)

---

## 🗄️ Structure de la base de données (extraits)

| Table                                                                                                                      | Description                                        |
| -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------- |
| `employe`                                                                                                                  | Infos RH (poste, salaire, embauche, téléphone)     |
| `plat`                                                                                                                     | Plats proposés : nom, prix, catégorie, ingrédients |
| `commande`                                                                                                                 | Commandes clients (sur place, livraison, etc.)     |
| `facture`                                                                                                                  | Paiement associé à chaque commande                 |
| `ingredient`                                                                                                               | Stock des produits utilisés                        |
| `fournisseur`                                                                                                              | Sources des produits alimentaires                  |
| `reserver`                                                                                                                 | Système de réservation (non encore utilisé)        |
| ![Capture d’écran du 2025-07-07 11-36-09](https://github.com/user-attachments/assets/7bec7b72-b424-41f3-9c17-720d4adbb7f8) |

---

## 🧾 Données clés extraites

- **Nombre total d’employés** : 12
- ![Capture d’écran du 2025-07-07 13-53-45](https://github.com/user-attachments/assets/a769b0da-41c4-4255-9f53-e5de245c1987)

- **Total des factures analysées** : 11
- ![Capture d’écran du 2025-07-05 11-38-51](https://github.com/user-attachments/assets/9dff9be5-1a2b-462f-8595-5ad3a3db3f0a)

- **Modes de paiement** : espèces, carte bancaire, Mobile Money
- **Commandes** : sur place, à emporter, livraison
- ![Capture d’écran du 2025-07-07 13-57-11](https://github.com/user-attachments/assets/f3bcfcbc-cb93-4642-b5c7-75783157c4b4)

- **Plats disponibles** : 12 (recettes locales et modernes)
  ![Capture d’écran du 2025-07-07 14-00-05](https://github.com/user-attachments/assets/f8aed715-b66a-414a-a6be-afeef46528cb)

- **Ingrédients suivis en stock** : 12 types (mil, sorgho, viande, etc.)
  ![Capture d’écran du 2025-07-07 13-56-14](https://github.com/user-attachments/assets/e1ed9419-ef9d-456f-8d39-d15ff2be9706)

---
---

## 🔧 Technologies utilisées

- **MariaDB 10+**
- **SQL**
- **Modélisation UML (AnalyseSI)**

---
## 🛠️ Étapes d’installation
### 1. 📁 Cloner le dépôt GitHub
```
     git clone https://github.com/ton-utilisateur/Ombre_Afrique_Abeche_Restaurant.git
     cd Ombre_Afrique_Abeche_Restaurant
```
## 🗃️ Créer la base de données dans MariaDB
### 2.Connecte-toi à MariaDB :
```
sudo mariadb -u root -p

```
### 3.Crée la base de données :
```
CREATE DATABASE ombr_afrique_dabeche CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;
EXIT;

```


## 📝 Auteurs

👨‍💻 Hissein Haroun Daoud  
📧 Contact : hisseindaoud6627@gmail.com  
🌍 Projet réalisé dans le cadre d’une formation en Developpement Web et Mobil– Abéché, Tchad WenakLabs et SimplonAfrica

---

## 📄 Licence

Ce projet est sous licence MIT. Vous pouvez le réutiliser et le modifier librement.

---

## 📌 Remarques

> 📌 **Note** : Le système est évolutif. Une version API REST (Express + Node.js) ou application de bureau (Electron) peut être développée à partir de ce modèle.
