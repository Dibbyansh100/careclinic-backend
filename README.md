# 🏥 CareClinic — Healthcare Appointment Management API

A Java Spring Boot REST API for managing doctors, patients, and healthcare appointments.

## 🛠️ Technology Stack

- **Backend:** Java 21, Spring Boot, Spring Security
- **Database:** PostgreSQL
- **ORM:** Spring Data JPA, Hibernate
- **Authentication:** JWT, role-based access control
- **API Documentation:** Swagger / OpenAPI

## ✨ Features

- Doctor and patient management
- Appointment booking, cancellation, and completion
- Validation of future appointment dates
- Application-level checks for doctor and patient scheduling conflicts
- JWT authentication and role-based API authorization
- Centralized exception handling
- PostgreSQL database integration

## 🔗 API Examples

| Method | Endpoint | Purpose |
|---|---|---|
| POST | `/api/v1/auth/register` | Register user |
| POST | `/api/v1/auth/login` | User login |
| POST | `/api/v1/appointments` | Book appointment |
| GET | `/api/v1/appointments` | List appointments |
| GET | `/api/v1/appointments/{id}` | Get appointment |
| GET | `/api/v1/appointments/patient/{patientId}` | Patient appointments |
| GET | `/api/v1/appointments/doctor/{doctorId}` | Doctor appointments |
| PATCH | `/api/v1/appointments/{id}/cancel` | Cancel appointment |
| PATCH | `/api/v1/appointments/{id}/complete` | Complete appointment |

Protected APIs require appropriate authentication and roles.

## 🚀 Run Locally

1. Install Java 21 and PostgreSQL.
2. Create a PostgreSQL database named `doctor_db`.
3. Configure database connection credentials using environment variables.
4. Configure a secure JWT signing secret through environment variables.
5. Run the application using `./mvnw spring-boot:run` on macOS/Linux or `.\mvnw.cmd spring-boot:run` on Windows.

The default application port is `8079`, unless overridden through configuration.

## 💻 Frontend Repository

[CareClinic React Frontend](https://github.com/Dibbyansh100/careclinic-frontend)

[Live Frontend Demo](https://doctor-appointment-project0-fronten.vercel.app/)

## 👨‍💻 Developer

Dibbyansh Pandey — Java Full Stack Developer
