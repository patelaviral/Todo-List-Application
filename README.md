# 📌 Full Stack Todo List Application
A simple and clean full-stack Todo List web application built using Spring Boot, Thymeleaf, Bootstrap, and MySQL.
This project demonstrates CRUD operations, MVC architecture, server-side rendering, and database integration.

# 🚀 Features
* Add new tasks
* Update existing tasks
* Delete tasks
* Mark tasks as completed / not completed
* Responsive UI using Bootstrap
* MySQL database integration
* Clean and simple Thymeleaf templates

# 🛠️ Tech Stack
Backend: Spring Boot (MVC, JPA, Hibernate)
Frontend: Thymeleaf, HTML, Bootstrap 5
Database: MySQL
Build Tool: Maven

# 📁 Project Structure
src/
 ├── main/
 │   ├── java/com/example/todo
 │   │    ├── controller/
 │   │    ├── service/
 │   │    ├── repository/
 │   │    └── model/
 │   └── resources/
 │        ├── templates/
 │        │     └── tasks.html
 │        └── application.properties

# 🔗 Endpoints Overview
![image alt](https://github.com/patelaviral/Todo-List-Application/blob/5785a0adf6a33a698109623a66e8a0d0d51c0869/endpoint_for_todo.png)
```
Method	Endpoint	           Description	                  Parameters	     Returns
GET	    /tasks	             Displays all tasks	            None	           tasks view
POST	  /tasks	             Creates a new task	            title (String)	 Redirect to /tasks
POST	  /tasks/{id}/update	 Updates task title by ID	      id, title	       Redirect to /tasks
GET	    /tasks/{id}/delete	 Deletes task by ID	            id	             Redirect to /tasks
GET	    /tasks/{id}/toggle	 Toggles task completed status	id	             Redirect to /tasks
```


# ⚙️ Setup Instructions
1️⃣ Clone the Repository
```
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2️⃣ Configure MySQL

Create database:
```
CREATE DATABASE todo_app;
```

Update application.properties:
```
spring.datasource.url=jdbc:mysql://localhost:3306/todo_app
spring.datasource.username=your_mysql_user
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
```

3️⃣ Run the Application

Use Maven or your IDE:
```
mvn spring-boot:run
```
4️⃣ Access in Browser
```
http://localhost:8080/tasks
```


📷 Screenshots
![image alt](https://github.com/patelaviral/Todo-List-Application/blob/5785a0adf6a33a698109623a66e8a0d0d51c0869/todo_application.png)
🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.
