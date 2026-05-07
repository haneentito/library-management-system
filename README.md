# Library Management System

A desktop-based Library Management System developed using Java Swing and MySQL following layered architecture and multiple design patterns.

---

## Features

- User Login & Signup
- Add New Books
- View All Books
- Delete Books
- Borrow Books
- Search Books
- Database Integration using MySQL
- GUI built with Java Swing

---

## Technologies Used

- Java
- Java Swing
- MySQL
- JDBC
- NetBeans IDE

---

## Design Patterns Implemented

### Singleton Pattern
Used in:
- `DBConnection`

Purpose:
- Ensure only one database connection instance exists.

---

### Factory Pattern
Used in:
- `UserFactory`
- `Admin`
- `Student`
- `Librarian`

Purpose:
- Create different user types dynamically.

---

### Strategy Pattern
Used in:
- `SearchStrategy`
- `SearchByTitle`
- `SearchByAuthor`
- `SearchByCategory`
- `SearchContext`

Purpose:
- Allow switching between different search algorithms dynamically.

---

### Observer Pattern
Used in:
- `Observer`
- `Subject`
- `NotificationService`
- `UserObserver`

Purpose:
- Notify users when borrowing operations occur.

---

### Facade Pattern
Used in:
- `LibraryFacade`

Purpose:
- Simplify communication between GUI and backend layers.

---

## Project Structure

```text
src/
 ├── dao/
 ├── facade/
 ├── factory/
 ├── gui/
 ├── model/
 ├── observer/
 ├── singleton/
 ├── strategy/
 └── main/
```

---

## Database

Database used:
- MySQL

Tables:
- users
- books
- borrow_records

---

## Screenshots

### Login Screen
![Login](screenshots/login.png)

### Dashboard
![Dashboard](screenshots/Dashboard.png)

### View Books
(Add screenshot here)

### Search Books
(Add screenshot here)

---

## How to Run

1. Clone repository

```bash
git clone https://github.com/haneentito/library-management-system.git
```

2. Open project in NetBeans

3. Create MySQL database

4. Configure database credentials inside:

```text
src/singleton/DBConnection.java
```

5. Run project

---

## Future Improvements

- Role-based authorization
- Return books feature
- Fine/payment system
- Export reports
- Dark mode UI
- Better search optimization
- Maven migration
- REST API version using Spring Boot

---

## Author

Haneen Tito  
Backend Developer
