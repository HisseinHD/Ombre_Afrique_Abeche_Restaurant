# 🍽️ Ombre Afrique d’Abéché - Système de Gestion de Restaurant

Bienvenue dans le dépôt officiel du projet **Ombre_Afrique_Abeche_Restaurant**, une solution complète de gestion pour un restaurant traditionnel basé à Abéché, Tchad.  
Ce projet s'appuie sur une base de données relationnelle MariaDB et propose une structure claire pour gérer les **employés**, **commandes**, **factures**, **plats**, **stocks**, et **réservations**.


![Capture d’écran du 2025-07-07 11-20-36](https://github.com/user-attachments/assets/52bbd738-1d46-4915-8360-b2a2616112b8)

![Capture d’écran du 2025-07-07 11-20-45](https://github.com/user-attachments/assets/a27792fb-0ed8-4dc0-83fa-a7ebeb64bb45)

---

## 📊 Objectif du projet

Ce projet vise à :
- Digitaliser les processus internes du restaurant (prise de commande, gestion des stocks, facturation)
- Suivre les performances (ventes, paiements, réservations)
- Améliorer la gestion des employés et des fournisseurs
- Proposer une base solide pour des extensions futures (application mobile, dashboard admin, etc.)

---

## 🧠 Modélisation de la base de données
### 1.Dicitionnaire de données 

![Capture d’écran du 2025-07-07 12-11-13](https://github.com/user-attachments/assets/55d6aab4-9fe4-4730-83a6-5a79ec141d60)

![Capture d’écran du 2025-07-07 12-11-28](https://github.com/user-attachments/assets/c62b93c4-db4d-401e-9f19-09ddae83b462)

### 2. 🧩 MCD – Modèle Conceptuel de Données  
![Capture d’écran du 2025-07-07 12-11-56](https://github.com/user-attachments/assets/5da63729-be0e-4db2-93f2-570974e635a1)


### 3. 🧩 MLD – Modèle Logique de Données  

![Capture d’écran du 2025-07-07 12-11-42](https://github.com/user-attachments/assets/1096271f-2998-4e30-a2c6-2720aeeb1ec4)

### 4. 🧩 MPD – Modèle Physique de Données (Script SQL)  

![Capture d’écran du 2025-07-05 11-43-16](https://github.com/user-attachments/assets/0adfd17e-23d8-4182-84dc-7e23cb9b44b5)

---

## 🗄️ Structure de la base de données (extraits)

| Table           | Description                                      |
|----------------|--------------------------------------------------|
| `employe`       | Infos RH (poste, salaire, embauche, téléphone)   |
| `plat`          | Plats proposés : nom, prix, catégorie, ingrédients |
| `commande`      | Commandes clients (sur place, livraison, etc.)   |
| `facture`       | Paiement associé à chaque commande               |
| `ingredient`    | Stock des produits utilisés                      |
| `fournisseur`   | Sources des produits alimentaires                |
| `reserver`      | Système de réservation (non encore utilisé)      |

---

## 🧾 Données clés extraites

- **Nombre total d’employés** : 12  
- **Total des factures analysées** : 11  
- **Modes de paiement** : espèces, carte bancaire, Mobile Money  
- **Commandes** : sur place, à emporter, livraison  
- **Plats disponibles** : 12 (recettes locales et modernes)  
- **Ingrédients suivis en stock** : 12 types (mil, sorgho, viande, etc.)

---

## 🧮 Exemple d'analyse disponible dans `/docs/rapport.md` ou `/docs/rapport.pdf`

- Analyse des commandes
- Fréquence des plats
- Répartition des paiements
- Statistiques salariales des employés
- Optimisation des stocks et fournisseurs

---

## 📂 Arborescence du projet





---

## 🔧 Technologies utilisées

- **MariaDB 10+**
- **SQL**
- **Modélisation UML (AnalyseSI)**

---

## 📝 Auteurs

👨‍💻 Hissein Haroun Daoud  
📧 Contact : hisseindaoud6627@gmail.com  
🌍 Projet réalisé dans le cadre d’une formation en Developpement Web et Mobil– Abéché, Tchad WenakLabs

---

## 📄 Licence

Ce projet est sous licence MIT. Vous pouvez le réutiliser et le modifier librement.

---

## 📌 Remarques

> 📌 **Note** : Le système est évolutif. Une version API REST (Express + Node.js) ou application de bureau (Electron) peut être développée à partir de ce modèle.



