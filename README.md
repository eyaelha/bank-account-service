# Bank Account Service

Micro-service REST développé avec **Spring Boot** permettant la gestion de comptes bancaires (création, consultation, mise à jour, suppression), avec persistance via **Spring Data JPA** et base de données **H2**.

## 🛠️ Technologies utilisées

- Java / Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database (base de données en mémoire)
- Lombok
- SpringDoc OpenAPI (Swagger UI)

## 📁 Structure du projet

- **Entité JPA** : `Compte` — représente un compte bancaire
- **Repository** : `CompteRepository` — interface Spring Data JPA pour l'accès aux données
- **Web Service RESTful** : `AccountRestController` — expose les opérations CRUD sur les comptes

## 🚀 Lancer le projet

```bash
mvn spring-boot:run
```

L'application démarre par défaut sur `http://localhost:8081`.

## 🗄️ Console H2

Accessible sur :
```
http://localhost:8081/h2-console
```

## 📑 Documentation API (Swagger)

Une fois l'application lancée, la documentation interactive est disponible sur :
```
http://localhost:8081/swagger-ui.html
```

## 🧪 Tester l'API

Le web service peut être testé avec un client REST comme **Postman** :
- `GET /comptes` — liste tous les comptes
- `GET /comptes/{id}` — récupère un compte par son id
- `POST /comptes` — crée un nouveau compte
- `PUT /comptes/{id}` — met à jour un compte
- `DELETE /comptes/{id}` — supprime un compte

## 📝 Contexte

Projet réalisé dans le cadre d'un exercice universitaire (ENSET) reprenant la démarche de création d'un micro-service de gestion de comptes bancaires avec Spring Boot.