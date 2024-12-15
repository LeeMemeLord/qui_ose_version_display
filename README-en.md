# Qui-Ose

Qui-Ose is a web application designed to help students find internships that match their study programs.

## Technologies Used

- **React**: Front-end
- **Java**: Back-end (Spring Boot)
- **PostgreSQL**: Database
- **JWT**: Security

---

## How to Run the Application

### 1. Install Dependencies

Clone the project repository from GitHub:
```bash
git clone <repository_url>
cd <project_name>
```

#### For the Front-end (React):
```bash
cd frontend
npm install
```

#### For the Back-end (Java):
Ensure Maven or Gradle is configured, then run:
```bash
mvn install
```

---

### 2. Configure the Database

- Install PostgreSQL.
- Create a dedicated database for the application.
- Update the configuration files in the **back-end** folder (e.g., `application.properties` or `application.yml`) with your database details:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/<database_name>
spring.datasource.username=<your_username>
spring.datasource.password=<your_password>
```

---

### 3. Start the Application

#### Start the Back-end Server (Spring Boot):
From the back-end folder, run:
```bash
mvn spring-boot:run
```
By default, the server will be available at **http://localhost:8080**.

#### Start the Front-end Server (React):
From the `frontend` folder, run:
```bash
npm start
```
The front-end application will be available at **http://localhost:3000**.

---

### 4. Connect and Use the Application

- Open the web interface (React) in your browser: [http://localhost:3000](http://localhost:3000).
- Sign up or log in to access the features:
  - **Search for internships**
  - **Submit applications**
  - **Manage student and employer profiles**

---

### 5. Deployment

To deploy the application to production, follow these steps:

#### Using Docker:
- Create `Dockerfile` and `docker-compose.yml` files to containerize the front end, back end, and database.

#### Hosting:
- Use a platform like **Heroku**, **AWS**, or **Google Cloud** to deploy your services.

---

### Best Practices

- **Updates**: Keep your dependencies (npm and Maven) up-to-date to avoid vulnerabilities.
- **Backups**: Regularly back up your PostgreSQL database.
- **Testing**: Test the application in different environments (development, production) before deployment.

---

## Author

Developed by Mikhail Kurilenko.
