# Smart Home Device Management

A comprehensive full-stack application designed to manage smart home devices and their categories. This project leverages a modern technology stack with Spring Boot for the backend and Angular for the frontend, fully containerized using Docker for easy deployment.

## 🏗 Architecture

The application is built using a microservices-ready architecture:

-   **Backend**: Spring Boot (Java 17) - Handles business logic, data persistence, and exposes REST APIs.
-   **Frontend**: Angular (with Tailwind CSS) - Provides a responsive and interactive user interface.
-   **Database**: MySQL - Relational database for storing device and category data.
-   **Database Management**: PhpMyAdmin - Web interface for managing the MySQL database.
-   **Containerization**: Docker & Docker Compose - Orchestrates the entire application stack.

## 🚀 features

-   **Category Management**: Create, read, update, and delete device categories.
-   **Device (Appareil) Management**: Manage smart home devices, including adding new devices, viewing details, updating status, and removing devices.
-   **Responsive Design**: Built with Tailwind CSS to ensure usability across different screen sizes.

## 🛠 Technologies Used

-   **Java 17**
-   **Spring Boot 3.x** (Spring Data JPA, Spring Web)
-   **Angular 16+**
-   **MySQL 8**
-   **Docker & Docker Compose**
-   **Maven** (Backend Build Tool)
-   **NPM** (Frontend Package Manager)

## 📋 Prerequisites

Before you begin, ensure you have the following installed on your machine:

-   [Docker Desktop](https://www.docker.com/products/docker-desktop)

## 🏎 Getting Started

Follow these steps to get the application up and running:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Sohaib-Laarichi/TP-24-Conteneurisation-Spring-Angular.git
    cd TP-24-Conteneurisation-Spring-Angular
    ```

2.  **Build and run the application:**
    Use Docker Compose to build the images and start the services.
    ```bash
    docker-compose up --build
    ```
    *Note: The first run might take a few minutes as it downloads necessary Docker images and builds the project artifacts.*

3.  **Access the Application:**

    -   **Frontend (User Interface):** [http://localhost:80](http://localhost:80)
    -   **Backend API:** [http://localhost:8085](http://localhost:8085)
    -   **PhpMyAdmin (Database Manager):** [http://localhost:8081](http://localhost:8081)
        -   **Username:** `root`
        -   **Password:** `root`

## 📂 Project Structure

-   `Smart_Home_back/`: Contains the Spring Boot backend source code.
-   `smartHome-front/`: Contains the Angular frontend source code.
-   `docker-compose.yml`: Defines the services, networks, and volumes for Docker.

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.
