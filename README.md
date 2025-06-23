# 🛒 E-Commerce Backend Project (Spring Boot)

A simple yet robust **E-Commerce backend** built using **Spring Boot**, designed to handle essential operations like product management, image upload, and search functionality. It follows a clean and modular architecture (Controller → Service → Repository) and uses **PostgreSQL** for persistent storage.

---

## 🚀 Features

- 🛍️ Product CRUD Operations (Add, Update, Delete, View)
- 🖼️ Image Upload & Retrieval via API
- 🔍 Keyword-based Product Search
- 🧼 Clean, maintainable Spring Boot architecture

---

## 🖥️ Sample Frontend

A sample frontend made using **React.js** is available in the [ecom-frontend-5](https://github.com/AnimeshNilawar/ecom-project-Spring/tree/main/ecom-frontend-5) folder.  
Use it to test and visualize the backend APIs in action.

---

## 🛠️ Tech Stack

| Layer        | Technology           | Icon |
|--------------|----------------------|------|
| Language     | Java                 | ![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=flat&logo=java&logoColor=white) |
| Framework    | Spring Boot          | ![Spring](https://img.shields.io/badge/SpringBoot-6DB33F?style=flat&logo=spring-boot&logoColor=white) |
| ORM          | Spring Data JPA      | ![JPA](https://img.shields.io/badge/JPA-007396?style=flat&logo=hibernate&logoColor=white) |
| Database     | PostgreSQL           | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) |
| Build Tool   | Maven                | ![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat&logo=apache-maven&logoColor=white) |
| API Standard | REST (Spring MVC)    | ![REST](https://img.shields.io/badge/REST-API-blue) |
| File Upload  | Multipart Support    | 📦 |

---

## 📁 Project Structure

```
ecom-project-Spring/
├── src/
│   ├── main/
│   │   ├── java/com/moddynerd/springecom/
│   │   │   ├── controller/
│   │   │   ├── model/
│   │   │   ├── repository/
│   │   │   ├── service/
│   │   │   └── SpringEcomApplication.java
│   │   └── resources/
│   │       ├── application.properties
└── pom.xml
```

---

## 🧪 API Endpoints

### 📦 Product APIs

| Method | Endpoint                          | Description                          |
|--------|-----------------------------------|--------------------------------------|
| GET    | `/api/products`                   | Get all products                     |
| GET    | `/api/product/{id}`               | Get a specific product by ID         |
| GET    | `/api/product/{productId}/image`  | Get product image as byte stream     |
| POST   | `/api/product`                    | Add new product with image           |
| PUT    | `/api/product/{id}`               | Update product by ID with new image  |
| DELETE | `/api/product/{id}`               | Delete product by ID                 |
| GET    | `/api/products/search?keyword=...`| Search products by keyword           |

> 📌 Use `multipart/form-data` for POST/PUT requests with product data and image.

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/AnimeshNilawar/ecom-project-Spring.git
cd ecom-project-Spring
```

### 2️⃣ Configure PostgreSQL

Update the `application.properties` file:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/demo
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.datasource.driver-class-name=org.postgresql.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.datasource.hikari.auto-commit=false
```

### 3️⃣ Run the Application

```bash
./mvnw spring-boot:run
```

### 4️⃣ Access API

Use Postman or your frontend to test endpoints:
- `http://localhost:8080/api/products`
- `http://localhost:8080/api/product/1`

---

## 👨‍💻 Author

| ![Animesh Nilawar](https://avatars.githubusercontent.com/AnimeshNilawar?s=100) |
|:--:|
| [**Animesh Nilawar**](https://github.com/AnimeshNilawar) |

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🌟 Show Your Support

Give this repo a ⭐ if you found it useful! Contributions are welcome via [pull requests](https://github.com/AnimeshNilawar/ecom-project-Spring/pulls).
