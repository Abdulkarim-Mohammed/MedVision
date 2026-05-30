# MedVision — AI-Powered Medical Diagnostics

MedVision is a web-based platform that allows users to upload medical scans and receive AI-powered diagnostic predictions. The system supports three types of medical image analysis in one place, making it faster and easier for healthcare use.

---

## Pages

### Login

The login page is the entry point of the MedVision system.  
Users must enter their **username** and **password** to access the platform.
<img width="999" height="814" alt="Screenshot 2026-05-31 013131" src="https://github.com/user-attachments/assets/7578ea9a-8fb7-4568-8b6f-1794e262b934" />

#### Features:
- Secure authentication using PHP sessions
- Input validation with error messages for invalid credentials
- Clean and responsive UI built with HTML & CSS
- Redirects to the main dashboard upon successful login

#### How to use:
1. Open `http://localhost/medvision/login.php`
2. Enter your username and password
3. Click the **Login** button to access the system

### Home
The landing page introduces the platform with a brief overview of its features: supports many scan types, delivers fast results, and keeps uploaded files private and secure.

![Home Page](screenshots/home.png)

---

### Analysis
Users can select one of three scan types, then upload the corresponding medical image to receive a prediction.

Supported scan types:
- Brain Tumor
- Disc Hernia
- Breast Cancer

Accepted format: MRI or CT scan (DICOM)

![Analysis Page](screenshots/analysis.png)

---

### About
Describes the mission and vision behind MedVision. The platform combines three AI models into a single interface to support medical image analysis with better accuracy and less time.

![About Page](screenshots/about.png)

---

### Contact
Provides contact information and a message form for users to reach out.

- Email: support@medvision.org
- Phone: +966 11 391 9000
- Address: As-Salam Road, Al Madinah Al Munawwarah

![Contact Page](screenshots/contact.png)

---

## Tech Stack

| Layer     | Technology        |
|-----------|-------------------|
| Frontend  | HTML, CSS, JavaScript |
| Backend   | PHP               |
| Database  | MySQL             |
| Server    | Apache (XAMPP)    |

---

## Project Structure

```
MedVision/
├── images/
├── index.php
├── analysis.php
├── about.php
├── contact.php
├── login.php
├── logout.php
├── script.js
└── style.css
```

## ⚙️ Installation

### Requirements
- [XAMPP](https://www.apachefriends.org/) (Apache + MySQL + PHP)
- Web Browser (Chrome, Firefox, Edge)

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/Abdulkarim-Mohammed/medvision-.git
```

**2. Move project to XAMPP folder**

Copy the project folder to:
C:\xampp\htdocs\medvision


**3. Start XAMPP**
- Open **XAMPP Control Panel**
- Start **Apache**
- Start **MySQL**

**4. Create the Database**
- Open your browser and go to: `http://localhost/phpmyadmin`
- Create a new database named: `medvision`
- Select the database and run the following SQL:

```sql
CREATE TABLE users (
    id        INT AUTO_INCREMENT PRIMARY KEY,
    username  VARCHAR(100) NOT NULL,
    password  VARCHAR(255) NOT NULL,
    fullname  VARCHAR(150) NOT NULL
);

INSERT INTO users (username, password, fullname)
VALUES ('admin', '1234', 'Admin User');
```

**5. Run the project**

Open your browser and go to:
http://localhost/medvision/login.php


**6. Login credentials**
| Field    | Value   |
|----------|---------|
| Username | admin   |
| Password | 1234    |

---
## Developed By MedVision Team | 2025
