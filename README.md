# Todo App Using Angular, Node and mysql

This project is created for TRIAS assignment. The frontend folder contains the Angular code and the backend folder contains the express code for the application.

## Setting Up

### Database
Create a database for this application
```bash
mysql -u <username> -p
```

```mysql
CREATE DATABASE todo_list_db;
USE todo_list_db;
CREATE TABLE tasks (
  id INT AUTO_INCREMENT PRIMARY KEY,
  title VARCHAR(255) NOT NULL,
  created_at TIMESTAMP,
  completed BOOLEAN DEFAULT 0
);

```

### Backend

Navigate to the backend folder and install the dependencies and run the code. U can access your backend api from http://localhost:3000/tasks

```bash
npm install
npm start
```

### Frontend

Navigate to the frontend folder and install the dependencies and run the code by passing proxy options. http://localhost:4200

```bash
npm install
ng serve --proxy-config src/proxy.conf.json
```

## Screenshots

### App Page
![Alt text](screenshots/image.png)

### Mat Dialog Box
![Alt text](screenshots/image-1.png)

### Update feature

![Alt text](screenshots/image-2.png)

### Database

![Alt text](screenshots/image-3.png)