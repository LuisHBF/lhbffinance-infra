# LHBFFinance Infrastructure

This repository contains the full infrastructure setup for the **LHBFFinance** platform — a personal finance system built with a microservices architecture, powered by Spring Boot, Kafka, Keycloak, and PostgreSQL.

---

## 🧰 Services included

| Service            | Description                                     | Port   |
|--------------------|-------------------------------------------------|--------|
| PostgreSQL (User)  | Database for user service and Keycloak          | 5433   |
| PostgreSQL (Finance) | Database for finance-related microservices   | 5434   |
| Keycloak           | Identity and access management                  | 8080   |
| Kafka              | Asynchronous communication between services     | 9092   |
| Zookeeper          | Kafka coordination service                      | 2181   |

---

## 🚀 How to run

Make sure you have **Docker** and **Docker Compose** installed.

```bash
docker-compose up -d
```

> This command will start all services in the background.

---

## 🔗 Useful URLs

- 🔐 **Keycloak Admin Console:**  
  [http://localhost:8080](http://localhost:8080)  
  - Username: `admin`  
  - Password: `admin`

---

## 🛠️ Database Access

You can connect using DBeaver, pgAdmin or any other SQL client.

### PostgreSQL – User Service

```
Host: localhost
Port: 5433
Database: user_db
User: user_service
Password: user_pass
```

### PostgreSQL – Finance Services

```
Host: localhost
Port: 5434
Database: finance_db
User: finance_service
Password: finance_pass
```

