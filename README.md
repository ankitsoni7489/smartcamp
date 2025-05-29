# CAMPso – Student Utility Web Portal 🎓📚

**CAMPso** is a full-stack web application designed to simplify university student life by integrating event scheduling, study planning, faculty directory, complaint management, lost & found, cafeteria menu, library search, note sharing, and important external links — all in one platform.

---

## 🌟 Features

### For Students
- **Event Scheduler:** View upcoming university events.
- **Study Planner:** Plan and organize daily study routines.
- **Faculty Directory:** Browse faculty contact details and locations.
- **Complaint Box:** Submit complaints and receive a tracking ID via email.
- **Lost & Found:** Report and claim lost or found items.
- **Cafeteria Menu:** Check daily menus of university shops.
- **Library System:** Search for book availability.
- **Note Sharing:** Upload and download class notes.
- **External Links:** Access important resources such as scholarships and academic portals.
- **Forgot Password:** Secure OTP-based password reset (valid for 2 minutes).

### Admin Panel
- Manage (Add/Update/Delete) events, faculty, students, complaints, notes, and external links.
- Validate and respond to complaints.
- Full control over the platform’s data and features.

---

## 🛠️ Tech Stack

- **Backend:** Java, Spring Boot, Spring Security, Spring Data JPA
- **Frontend:** HTML (Thymeleaf), CSS, JavaScript
- **Database:** MySQL
- **Email Service:** Java Mail Sender for OTP and complaint tracking emails

---

## 📂 Project Structure

src/
├── main/
│ ├── java/ (Java source code)
│ ├── resources/
│ ├── static/ (CSS, JS, images)
│ ├── templates/ (Thymeleaf HTML pages)
│ ├── application.properties (config file)
└── test/ (unit and integration tests)


---

## 🚀 Setup & Installation

### Prerequisites
- Java 17 or higher installed
- Maven installed
- MySQL Server installed and running
- IDE like IntelliJ IDEA or Eclipse (optional but recommended)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/campso.git
   cd campso
Configure database

2. Create a MySQL database, e.g., campso_db.

Update src/main/resources/application.properties with your MySQL username, password, and database URL:
spring.datasource.url=jdbc:mysql://localhost:3306/campso_db
spring.datasource.username=your_db_username
spring.datasource.password=your_db_password
Configure email credentials (for Java Mail Sender)

3. Add your SMTP email credentials to application.properties:

spring.mail.host=smtp.your-email-provider.com
spring.mail.port=587
spring.mail.username=your_email@example.com
spring.mail.password=your_email_password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true

4. Build and run the project
   mvn clean install
   mvn spring-boot:run

5. Access the application
   Open your browser and go to http://localhost:8080/login

