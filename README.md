# expert-invention
Code de Gestion de parc automobile
# Gestion de Parc Automobile

## Description
Cette application console permet à une entreprise de location de gérer son parc de véhicules, incluant différentes catégories de véhicules, les locations, ainsi que les informations clients. Ce projet utilise les concepts fondamentaux de la programmation orientée objet (POO) comme l'héritage, le polymorphisme, l'encapsulation, et la gestion des exceptions.

## Fonctionnalités
-"Gestion des véhicules" : Ajout de véhicules dans le parc, avec des attributs spécifiques pour les voitures et les camions.
- "Gestion des clients" : Enregistrement des informations clients et suivi des locations en cours.
- "Location et retour de véhicules": Louer un véhicule à un client et changer son statut, puis le retourner pour le rendre disponible.
- "Affichage" : Liste des véhicules disponibles ou loués.
- "Gestion des exceptions" : Vérification de la disponibilité des véhicules et validation des informations clients.

## Structure du Projet
Le projet est organisé en plusieurs classes principales :

- "Vehicule" : Classe de base abstraite représentant un véhicule.
  - **Attributs** : `immatriculation`, `marque`, `modele`, `anneeService`, `kilometrage`, `estLoue`.
  - **Méthodes** : `calculerPrixLocation()` (méthode abstraite pour le calcul du prix de location), `isDisponible()`.

- `Voiture` : Sous-classe de `Vehicule` représentant les voitures, avec des attributs spécifiques (`nombrePlaces`, `typeCarburant`).
- `Camion` : Sous-classe de `Vehicule` représentant les camions, avec des attributs spécifiques (`capaciteChargement`, `nombreEssieux`).

- `Client` : Classe pour les clients de l'entreprise, avec des informations personnelles (`nom`, `prenom`, `numeroPermis`, `telephone`) et une liste de locations en cours.

- `Louable` : Interface définissant les méthodes `louer()` et `retourner()` implémentées par les classes `Voiture` et `Camion`.

- `ParcAutomobile` : Classe pour stocker les véhicules dans une collection et gérer leur état (disponible ou loué).

- "Exceptions personnalisées":
  - "VehiculeIndisponibleException` : Exception levée lorsqu'un véhicule est déjà loué.
  - "ClientNonAutoriseException` : Exception levée si un client n'est pas autorisé à louer un camion sans permis adéquat.

## Prérequis
- Java 8 ou version supérieure
- IntelliJ IDEA
  

## Installation
1. **Cloner le dépôt Git** :
   https://github.com/assohounmarc8/expert-invention.git
