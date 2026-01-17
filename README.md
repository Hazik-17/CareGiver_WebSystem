# CareGiver WebSystem

A simple Jakarta EE web application for managing caregiver booking flows and basic user authentication. This repository contains a small demo/demo-class project implemented with Jakarta EE (REST resources, JPA persistence and plain HTML frontend pages).

**Purpose**
- Provide a minimal, educational example of a caregiver booking web application built with Jakarta EE 10.
- Demonstrate REST endpoints, persistence configuration, and a basic web UI (login, register, booking pages).

**Why this was developed**
- Learning / teaching: to explore Jakarta EE 10 features and how to structure a small webapp.
- Reference/demo for deploying a Java web application (WAR) with REST and JPA to a Jakarta-compatible server.

**Features (example)**
- User registration and login pages (`webapp/login.html`, `webapp/register.html`).
- Booking UI (`webapp/booking.html`) for creating/viewing appointments.
- Jakarta REST resource examples under `src/main/java/com/mycompany/caregiver/resources`.
- JPA persistence configured via `src/main/resources/META-INF/persistence.xml`.

**Tech stack**
- Java + Jakarta EE 10 (Jakarta REST, JPA)
- Maven for build (`pom.xml`)
- Any Jakarta EE 10 compatible servlet container or application server (Tomcat 10.1+, Payara, WildFly with Jakarta support)

**Quick start**
Prerequisites:
- Java 17+ (or the Java version required by the `pom.xml`)
- Maven
- A Jakarta EE 10 compatible server to deploy the generated WAR

Build and deploy:
1. Build the WAR:

```bash
mvn clean package
```

2. Deploy the produced `target/*.war` to your Jakarta EE 10 compatible server (for example, place the WAR in Tomcat's `webapps` folder).

3. Open the application in a browser and use the provided `login.html`, `register.html`, and `booking.html` pages.

**Project structure (important locations)**
- `src/main/java` — Java source code (REST resources and configuration)
- `src/main/resources/META-INF/persistence.xml` — JPA persistence configuration
- `src/main/webapp` — web UI files (HTML pages, WEB-INF)

**Next steps / notes**
- This project is a small starting point; add authentication, validation, database setup, and unit/integration tests for production use.
- If you want, I can: run a quick code scan, add a CONTRIBUTING section, or create a small Dockerfile for easier local runs.

