# Les14
# NoSQL

## 1) Створення бази даних та колекцій:

### Назвіть базу даних як gymDatabase
use gymDatabase

switched to db gymDatabase
### Створіть колекції: clients, memberships, workouts, trainers

## 2) Визначення схеми документів:
### Clients: client_id, name, age, email

db.clients.insertOne({"client_id": "40", "name": "Arnold Iron", "email": "arnold@example.com", "age": "75"})

db.clients.insertOne({"client_id": "23", "name": "Alex Albon", "email": "alex.albon@example.com", "age": "29"})

db.clients.insertOne({"client_id": "3", "name": "Ann Smith", "email": "ann.smith@example.com", "age": "25"})

db.clients.insertOne({"client_id": "2", "name": "Will Smith", "email": "will.smith@example.com", "age": "30"})

db.clients.insertOne({"client_id": "1", "name": "Jacky Chang", "email": "jane.smith@example.com", "age": "60"})

### Memberships: membership_id, client_id, start_date, end_date, type

db.memberships.insertOne({"Membership_id": "1", "client_id": "1", "start_date": "2024-10-01", "end_date": "2025-01-01" ,"type": "Premium"})

db.memberships.insertOne({"Membership_id": "2", "client_id": "2", "start_date": "2024-09-01", "end_date": "2025-01-01" ,"type": "Premium"})

db.memberships.insertOne({"Membership_id": "3", "client_id": "3", "start_date": "2024-01-01", "end_date": "2025-01-01" ,"type": "Premium"})

db.memberships.insertOne({"Membership_id": "23", "client_id": "23", "start_date": "2024-09-19", "end_date": "2025-01-01" ,"type": "Basic"})

db.memberships.insertOne({"Membership_id": "40", "client_id": "40", "start_date": "2024-09-20", "end_date": "2024-11-01" ,"type": "Basic"})

### Workouts: workout_id, description, difficulty
db.workouts.insertOne({"Workout_id": "11", "description": "running", "difficulty": "Easy"})

db.workouts.insertOne({"Workout_id": "99", "description": "Strength Training", "difficulty": "High"})

db.workouts.insertOne({"Workout_id": "44", "description": "Cardio Training", "difficulty": "Medium"})

### Trainers: trainer_id, name, specialization

db.trainers.insertOne({"trainer_id": "101", "name": "Toto Wolf", "email": "toto.wolf@example.com", "age": "50"})

db.trainers.insertOne({"trainer_id": "102", "name": "Leonel Messi", "email": "messi@example.com", "age": "38"})

db.trainers.insertOne({"trainer_id": "103", "name": "Mickel Falbs", "email": "falbs@example.com", "age": "48"})

## 3) Заповнення колекцій даними:
### Додайте кілька записів до кожної колекції

## 4) Запити:
### Знайдіть всіх клієнтів віком понад 30 років
### Перелічіть тренування із середньою складністю
### Покажіть інформацію про членство клієнта з певним client_id
