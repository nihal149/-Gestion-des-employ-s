 Gestion des Employés
 
 Description :

Ce projet est une application de gestion des employés dans une petite entreprise. Il permet de modéliser une hiérarchie d'employés, composée d'un directeur général, d'un manager, et de développeurs. L'application gère les informations des employés (noms, salaires) et les affiche selon leur position dans la hiérarchie. Elle utilise Java et JDBC pour interagir avec une base de données MySQL et permet d'effectuer des opérations de création, lecture, mise à jour et suppression (CRUD) des données.

Structure du Projet:

- Connexion à la base de données : Une classe `Connexion` a été créée pour établir une connexion à une base de données MySQL à l'aide des informations de connexion définies dans le fichier de configuration `base.properties`.
  
- Modélisation des employés : Les employés sont représentés par des classes `Personne`, `Manager`, et `Developpeur`, qui reflètent la hiérarchie de l'entreprise. Ces classes permettent de stocker les informations des employés comme le nom et le salaire.

- Interface DAO : L'interface `IDao` a été définie pour assurer les opérations CRUD sur les objets employés. Elle est implémentée par les classes de service.

- Services CRUD: Les classes `ManagerService` et `DeveloppeurService` implémentent l'interface `IDao` et fournissent les méthodes nécessaires pour gérer les données des employés dans la base de données.

- Test de l'application : Une classe `Entreprise` permet de tester le système en créant des employés, en établissant les relations hiérarchiques, et en affichant les informations de chaque employé du plus haut au plus bas dans la hiérarchie.

 Fonctionnalités:

- Connexion à une base de données MySQL pour gérer les informations des employés.
- Gestion d'une hiérarchie d'employés avec des relations entre directeur, manager et développeurs.
- Affichage des noms et des salaires des employés en fonction de leur position dans l'organisation.
- Opérations CRUD pour ajouter, consulter, modifier, et supprimer les informations des employés dans la base de données.

 Utilisation :

L'application simule une petite entreprise avec une hiérarchie simple. Après avoir configuré la base de données et lancé l'application, elle permet de :

- Créer des employés (directeur, manager, développeurs).
- Associer des développeurs à un manager, et le manager à un directeur.
- Afficher la hiérarchie et les salaires des employés de manière structurée.
  
 Auteurs:

Ce projet a été développé dans le cadre d'un exercice pédagogique visant à renforcer les compétences en programmation orientée objet avec Java et en gestion de bases de données via JDBC.

