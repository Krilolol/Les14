# Les14
# NoSQL

## 1) Створення бази даних та колекцій:

### Назвіть базу даних як gymDatabase
use gymDatabase

switched to db gymDatabase
### Створіть колекції: clients, memberships, workouts, trainers

## 2) Визначення схеми документів:
### Clients: client_id, name, age, email

db.clients.insertOne({"client_id": "40", "name": "Arnold Iron", "email": "arnold@example.com", "age": 75})

db.clients.insertOne({"client_id": "23", "name": "Alex Albon", "email": "alex.albon@example.com", "age": 29})

db.clients.insertOne({"client_id": "3", "name": "Ann Smith", "email": "ann.smith@example.com", "age": 25})

db.clients.insertOne({"client_id": "2", "name": "Will Smith", "email": "will.smith@example.com", "age": 30})

db.clients.insertOne({"client_id": "1", "name": "Jacky Chang", "email": "jane.smith@example.com", "age": 60})

![clients](https://github.com/user-attachments/assets/24533f1f-1df4-4678-a625-d5f4d816533b)

### Memberships: membership_id, client_id, start_date, end_date, type

db.memberships.insertOne({"Membership_id": "1", "client_id": "1", "start_date": "2024-10-01", "end_date": "2025-01-01" ,"type": "Premium"})

db.memberships.insertOne({"Membership_id": "2", "client_id": "2", "start_date": "2024-09-01", "end_date": "2025-01-01" ,"type": "Premium"})

db.memberships.insertOne({"Membership_id": "3", "client_id": "3", "start_date": "2024-01-01", "end_date": "2025-01-01" ,"type": "Premium"})

db.memberships.insertOne({"Membership_id": "23", "client_id": "23", "start_date": "2024-09-19", "end_date": "2025-01-01" ,"type": "Basic"})

db.memberships.insertOne({"Membership_id": "40", "client_id": "40", "start_date": "2024-09-20", "end_date": "2024-11-01" ,"type": "Basic"})
![memberships](https://github.com/user-attachments/assets/aa537251-6e51-49d4-868c-47cbd885bf3b)

### Workouts: workout_id, description, difficulty
db.workouts.insertOne({"Workout_id": "11", "description": "running", "difficulty": "Easy"})

db.workouts.insertOne({"Workout_id": "99", "description": "Strength Training", "difficulty": "High"})

db.workouts.insertOne({"Workout_id": "44", "description": "Cardio Training", "difficulty": "Medium"})
![workouts](https://github.com/user-attachments/assets/e6ed9e5c-1b85-4741-9636-3b5f3bd6f020)

### Trainers: trainer_id, name, specialization

db.trainers.insertOne({"trainer_id": "101", "name": "Toto Wolf", "email": "toto.wolf@example.com", "age": 50})

db.trainers.insertOne({"trainer_id": "102", "name": "Leonel Messi", "email": "messi@example.com", "age": 38})

db.trainers.insertOne({"trainer_id": "103", "name": "Mickel Falbs", "email": "falbs@example.com", "age": 48})
![trainers](https://github.com/user-attachments/assets/5461694a-6a58-4900-a888-9e1cd9fb558d)

##  Запити:
### Знайдіть всіх клієнтів віком понад 30 років
![client-30](https://github.com/user-attachments/assets/6b100314-5826-4e9d-9909-4cd88cb8b283)

### Перелічіть тренування із середньою складністю
![Medium](https://github.com/user-attachments/assets/0ca9f5ac-2ee3-4ed6-a0f4-8b3efe604fc6)

### Покажіть інформацію про членство клієнта з певним client_id
![membership-23](https://github.com/user-attachments/assets/44d77333-0b9d-4cfc-896d-e7d4d1594ab7)

