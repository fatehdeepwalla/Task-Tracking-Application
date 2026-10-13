
# Task Tracking Application

A secure full stack task tracking web application built with Spring Boot, Spring MVC, JSP, Spring Security, Spring Data JPA, H2.

The application features user authentication, Todo CRUD operations, form validation, and database persistence.

---

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Backend Framework** | Java \| Spring Boot \| Spring MVC |
| **Security** | Spring Security |
| **Persistence Layer** | Spring Data JPA \| Hibernate |
| **Database** | H2 In-Memory Database |
| **Frontend Templates** | JSP (JavaServer Pages) \| JSTL |
| **UI & Styling** | Bootstrap 5 \| jQuery |
| **Build Tooling** | Apache Maven |
| **Containerization** | Docker |

---

## ✨ Key Features

* **Authentication**: Secure authentication powered by Spring Security using standard form logins.
* **Full Task Lifecycle (CRUD)**: Create, view, update, and delete personal todo items bound to individual logged-in user sessions.
* **Data Validation**: Server-side field validation to ensure valid description lengths and completion dates before saving.
* **Responsive UI**: Built with Bootstrap 5 templates and interactive datepickers for accurate target date management.
* **JPA Persistence**: Automatic table schema generation and entity mapping via Spring Data JPA backed by H2.
* **Automated Seeding**: Pre-loaded startup data populated automatically using custom SQL scripts.
* **Docker Support**: Includes a Dockerfile for building and running the application as a container without requiring Java or Maven to be installed on the host machine.

---

## 🚀 Quick Start Guide

### Option 1: Run using Docker
- Prerequisites
   * Docker Desktop installed and running
   * No Java or Maven installation required
     
- Run the Pre-built Docker Image in container:
  ```bash
  docker container run -p 8080:8080 --name todo-app-container fatehdeepwalla/todo-app:v1
  ```
  > **Note:** A Dockerfile is included in the project for users who prefer to build the Docker image locally instead of using the pre-built image available on Docker Hub.

### Option 2: Run locally using the Source Code or Packaged WAR File
- Prerequisites
   * JDK 17 or higher
   * No Maven installation required, as maven wrapper is included

- Clone Repository
    ```bash
    git clone https://github.com/fatehdeepwalla/Task-Tracking-Application.git
    cd Task-Tracking-Application
    ```
    
- Run directly from source code Using Maven Wrapper
  ```bash
  ./mvnw spring-boot:run 
  ```
  
- Build and run packaged WAR file:
  ```bash
  ./mvnw clean package 
  java -jar target/ToDo_APP-0.0.1-SNAPSHOT.war
  ```

  > **Note:** For your convenience, the pre-built .war file is provided below, so you can run the application directly without building the project yourself.<br>
  > **Download:** [Download the pre-built WAR ⬇️](ToDo_APP-0.0.1-SNAPSHOT.war)

---

## 🖥️ Accessing the Application

- 🌐 Web Dashboard: `http://localhost:8080`
- 🔐 Application Login:
  
  | Credential | Details |
  | :--- | :--- |
  | **Username** | `admin` |
  | **Password** | `admin` |
- 🗄️ H2 Database Console: `http://localhost:8080/h2-console`
- ⚙️ Console Credentials & Settings:
  
   | Credential | Details |
   | :--- | :--- |
   | **JDBC URL** | `jdbc:h2:mem:testdb` |
   | **Username** | `sa` |
   | **Password** | *(Leave empty)* |

