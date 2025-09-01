Content Management For a Blog.java

This is a simple Content Management System (CMS) for a Blog, built using Spring Boot, Spring Data JPA, and H2 Database.
It provides REST APIs to manage Users, Blog Posts, and Comments.

🚀 Features

User management (create and list users)

Blog posts (create, update, list, search, publish/unpublish)

Comments (add, list, approve/reject)

In-memory H2 database with web console

RESTful API design with JSON responses

Simple validation for input data

📦 Tech Stack

Java 17

Spring Boot 3.x

Spring Data JPA

H2 In-Memory Database

Maven

⚙️ Setup & Run
Prerequisites

Java 17+ installed

Maven installed

Steps

Clone or unzip the project folder

Navigate to the project root

Run the application:

mvn spring-boot:run


The application starts on http://localhost:8080

H2 Database Console

Visit: http://localhost:8080/h2

JDBC URL: jdbc:h2:mem:blogdb

User: sa

Password: (empty)

📖 Example API Usage
1. Create a User
POST /api/users
Content-Type: application/json

{
  "username": "admin",
  "fullName": "Admin User",
  "email": "admin@example.com",
  "password": "secret"
}

2. Create a Blog Post
POST /api/posts
Content-Type: application/json

{
  "title": "My First Blog",
  "content": "This is my first blog post.",
  "tags": ["intro", "hello"],
  "publish": true,
  "authorId": 1
}

3. List Blog Posts
GET /api/posts

4. Search Blog Posts
GET /api/posts/search?q=blog

5. Add a Comment
POST /api/comments
Content-Type: application/json

{
  "postId": 1,
  "authorName": "Jane",
  "body": "Great post!"
}

6. Approve/Reject a Comment
PATCH /api/comments/{id}/approve?approved=true

✅ Future Enhancements

Add authentication & role-based access (Admin, Editor, Reader)

Deploy to cloud (Heroku, AWS, Azure)

Frontend UI with React or Angular

Analytics dashboard for blog traffic

Reach out! ✉️
Name: Ashika M
Email: ashikasjcetcse@gmailcom
GitHub: https://github.com/ashika67

Would you like me to bundle this README.md into the blog-cms.zip file I generated earlier so you have everything (code + docs) in one package?

You said:
