# TP – API Star Wars (SWAPI)

Documentation : https://swapi.tech/documentation

---

# Q1 – Est-ce une API publique ou privée ?

L’API **SWAPI (Star Wars API)** est une **API publique**.

## Justification

- La documentation est accessible librement sur internet.
- La rubrique **Authentification** indique qu’aucune authentification n’est nécessaire.
- Les requêtes peuvent être effectuées sans clé API ni token.

➡️ Donc, il s’agit d’une **API publique accessible en lecture**.

---

# Q2 – Liste des ressources disponibles

Les ressources disponibles dans l’API SWAPI sont :

- `people` → personnages
- `planets` → planètes
- `films` → films
- `species` → espèces
- `vehicles` → véhicules
- `starships` → vaisseaux spatiaux

Exemple de requête :


GET https://www.swapi.tech/api/people


---

# Q3 – Attributs d’un personnage et d’une planète

## Attributs d’un personnage (people)

- name
- height
- mass
- hair_color
- skin_color
- eye_color
- birth_year
- gender
- homeworld
- films
- species
- vehicles
- starships
- created
- edited
- url

---

## Attributs d’une planète (planets)

- name
- rotation_period
- orbital_period
- diameter
- climate
- gravity
- terrain
- surface_water
- population
- residents
- films
- created
- edited
- url

---

# Q4 – Informations sur Obi-Wan Kenobi

## Formulation de la réponse

### Verbe HTTP


GET


### Requête


https://www.swapi.tech/api/people/?name=obi-wan%20kenobi


### Code HTTP renvoyé


200 OK


### Format de réponse


JSON


---

## Résultat

### Description

- Nom : Obi-Wan Kenobi
- Genre : Masculin
- Taille : 182 cm
- Couleur des yeux : bleu
- Couleur des cheveux : auburn

---

### Films dans lesquels il apparaît

- The Phantom Menace
- Attack of the Clones
- Revenge of the Sith
- A New Hope
- The Empire Strikes Back
- Return of the Jedi

---

### Véhicules utilisés

- Tribubble Bongo

---

### Vaisseaux spatiaux

- Jedi Starfighter
- Trade Federation cruiser

---

### Planète natale

La planète natale est Stewjon.

---

# Q5 – Climat de la planète Tatooine

## Requête


GET https://www.swapi.tech/api/planets/?name=tatooine


## Code HTTP


200 OK


## Format de réponse


JSON


## Résultat

Climat :


arid


➡️ La planète **Tatooine possède un climat aride (désertique)**.

---

# Q6 – Vitesse et classe d’un Snowspeeder

## Requête


GET https://www.swapi.tech/api/vehicles/?name=snowspeeder


## Code HTTP


200 OK


## Format de réponse


JSON


## Résultat

Vitesse maximale :


650 km/h


Classe :


airspeeder


---

# Q7 – Hyperdrive d’un Star Destroyer

## Requête


GET https://www.swapi.tech/api/starships/?name=star%20destroyer


## Code HTTP


200 OK


## Format de réponse


JSON


## Résultat

Hyperdrive rating :


2.0


Films :

- A New Hope
- The Empire Strikes Back
- Return of the Jedi
- Revenge of the Sith
- Rogue One

---

# Q8 – Les droïdes

## Classification

Les droïdes sont classés dans :


species


Classification :


artificial


---

## Personnages droïdes

- C-3PO
- R2-D2
- BB-8

---

## Films où ils apparaissent

- A New Hope
- The Empire Strikes Back
- Return of the Jedi
- The Phantom Menace
- Attack of the Clones
- Revenge of the Sith
- The Force Awakens

---

# Q9 – Analyse de la requête GitHub

### Verbe HTTP


GET


### Requête


https://api.github.com/users/Kadaaran


---

## Que représente "Kadaaran" ?

C’est le **nom d’utilisateur GitHub**.

---

## URL


https://api.github.com/users/Kadaaran


---

## Nom de domaine


api.github.com


---

## URI


/users/Kadaaran


---

## Nom et prénom de l’utilisateur


Kassandre Pedro


---

## Ville


Lyon


---

# Q10 – Comment savoir si une API est fiable ?

Pour vérifier la fiabilité d’une API :

- présence d’un **système d’authentification**
- **autorisation des accès**
- **utilisation du protocole HTTPS**
- **documentation claire**
- **mises à jour régulières**

Exemple :

Historique des commits de PokeAPI :

https://github.com/PokeAPI/pokeapi/commits/master/

---

# Q11 – Token d’authentification GitHub

## a) Qu’est-ce qu’un token d’authentification ?

Un **token d’authentification** est une **clé secrète générée par un service** permettant à un utilisateur ou une application :

- de s’authentifier auprès d’une API
- d’accéder à certaines fonctionnalités
- d’effectuer des actions sécurisées

Il remplace généralement le mot de passe pour les requêtes API.

---

## b) Génération d’un token

Étapes :

1. Aller sur :


https://github.com/settings/tokens


2. Cliquer sur :


Generate new token


3. Choisir :


for general use


4. Dans **Note**, écrire :


LSW BTS SIO1 IA


5. Cocher les permissions :


repo
delete_repo


6. Cliquer sur :


Generate token


7. Copier et conserver le token généré.

**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**