# RAMSY Medical Laboratories – Front Desk & Queue Management System

## Overview

The **RAMSY Medical Laboratories Front Desk & Queue Management System** is a desktop healthcare application developed using **Python**, **Tkinter**, and **MySQL**. The system is designed to streamline patient registration, queue management, appointment scheduling, and health worker assignment within a medical laboratory or clinic.

The application automates patient flow by prioritizing emergency cases, assigning healthcare workers based on specialization and workload, and maintaining patient records in a MySQL database. By replacing manual processes with an efficient digital solution, the system helps reduce waiting times, improve service delivery, and enhance patient satisfaction.

This project was developed as part of the **PROG103 – Principles of Structured Programming** course at **Limkokwing University of Creative Technology – Sierra Leone**.

---
## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [How the System Works](#how-the-system-works)
- [Database](#database)
- [Structured Programming Concepts](#structured-programming-concepts)
- [Installation](#installation)
- [Future Enhancements](#future-enhancements)
- [Sustainable Development Goal](#sustainable-development-goal)
- [Screenshots](#screenshots)
- [License](#license)
- [Authors](#authors)
- [Acknowledgements](#acknowledgements)
- [Support](#support)


## Problem Statement

Many healthcare facilities in Sierra Leone still rely on manual systems for patient registration and queue management. These methods often result in:

- Long patient waiting times
- Poor prioritization of emergency cases
- Misplaced or incomplete patient records
- Increased workload for healthcare staff
- Inefficient appointment scheduling
- Reduced patient satisfaction

The RAMSY Medical Laboratories Front Desk & Queue Management System addresses these challenges by providing a digital platform for managing patients, appointments, and healthcare staff efficiently.

---

## Objectives

The project aims to:

- Automate patient registration and queue management
- Prioritize emergency patients based on symptoms and age
- Reduce patient waiting times
- Improve clinic efficiency and workflow
- Demonstrate structured programming concepts using Python
- Support Sustainable Development Goal (SDG) 3: Good Health and Well-Being

---

## Features

### Patient Registration

- Register patients with personal and contact information
- Record date of birth, gender, address, and emergency contact
- Capture patient symptoms for automatic priority classification

### Queue Management

- Automatic queue number generation
- Priority-based queue sorting
- Real-time queue display
- Patient search functionality
- Serve patients in priority order

### Appointment Scheduling

- Book appointments for registered patients
- Prevent scheduling appointments in the past
- Automatic appointment reminders
- Link appointments directly to patient records

### Priority Classification

Patients are automatically categorized into one of the following priority levels:

- Emergency
- High Priority
- Normal

Priority is determined using patient symptoms and age.

### Health Worker Assignment

- Automatically assign healthcare workers based on specialization
- Balance workloads among available staff
- Fallback assignment to General Practitioners when necessary

### System Functions

- Add Patient
- View Queue
- Serve Patient
- Clear Queue
- Export Queue to Text File
- Exit Application

---

## Technologies Used

- Python 3.x
- Tkinter
- MySQL
- mysql-connector-python
- Pillow (PIL)

---

## Project Structure

```text
RAMSY-Medical-Laboratories/
│
├── front_desk_app.py
├── database.py
├── queue_manager.py
├── requirements.txt
├── README.md
├── LICENSE
└── assets/
```

---

## How the System Works

1. Register a new patient by entering personal information and symptoms.
2. The system automatically determines the patient's priority level.
3. A queue number is assigned.
4. The patient is added to the queue according to priority.
5. If an appointment is required, the system schedules it and assigns an appropriate healthcare worker.
6. Healthcare staff serve patients based on queue priority.
7. Queue information is updated automatically after each patient is served.

---

## Database

The application uses a MySQL database to manage:

- Patient records
- Appointment information
- Healthcare worker information
- Queue records

---

## Structured Programming Concepts

This project demonstrates the practical application of structured programming through:

- Variables and Constants
- Data Types
- Decision Structures (`if`, `elif`, `else`)
- Loops
- User-Defined Functions
- Input Validation
- Lists and Dictionaries
- Modular Programming

### Main Functions

- `determine_priority()`
- `add_patient_to_queue()`
- `display_queue_window()`
- `serve_patient()`
- `clear_queue()`
- `match_diagnosis()`
- `assign_specialty()`

---

## Installation

### Prerequisites

Ensure the following are installed:

- Python 3.x
- MySQL Server

### Install Dependencies

```bash
pip install -r requirements.txt
```

If you do not have a `requirements.txt` file, install the required packages manually:

```bash
pip install mysql-connector-python pillow
```

### Clone the Repository

```bash
git clone https://github.com/your-username/ramsy-medical-laboratories.git
```

### Navigate to the Project Directory

```bash
cd ramsy-medical-laboratories
```

### Configure the Database

Update the `DB_CONFIG` settings in the application with your MySQL credentials:

- Host
- Username
- Password
- Database Name

### Run the Application

```bash
python front_desk_app.py
```

---

## Future Enhancements

Future versions of the system may include:

- SMS and email appointment notifications
- Cloud deployment for multi-user access
- Electronic medical record integration
- Advanced patient search and filtering
- Analytics dashboard for patient flow
- Reporting and data visualization
- Role-based user authentication
- Online appointment booking

---

## Sustainable Development Goal

This project supports **United Nations Sustainable Development Goal 3 – Good Health and Well-Being** by:

- Improving healthcare efficiency
- Reducing patient waiting times
- Prioritizing emergency cases
- Enhancing patient management
- Supporting faster healthcare delivery

---

## Screenshots

## Application Preview

Below are screenshots showcasing the main features of the application.

### Landing Page

The landing page introduces the platform and provides quick access to the main sections.

![Landing Page](images/home.png)

### Dashboard

The dashboard displays key information and provides easy navigation to all system features.

![Dashboard](images/dashboard.png)

### Profile Page

Users can view and update their personal information from the profile page.

![Profile](images/profile.png)

---

## License

This project is licensed under the **MIT License**.

Copyright (c) 2026 Lisa Kadija Abass Wurie, Charles Nyakeh Ensah, and Donald Sheku.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and its associated documentation files to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, subject to the conditions of the MIT License.

See the **LICENSE** file for the complete license text.
---

## Authors

Developed by:

- **Lisa Kadija Abass Wurie**
- **Charles Nyakeh Ensah**
- **Donald Sheku**

**Course:** PROG103 – Principles of Structured Programming

**Institution:** Limkokwing University of Creative Technology – Sierra Leone

---

## Acknowledgements

The authors would like to thank:

- Limkokwing University of Creative Technology – Sierra Leone
- The PROG103 lecturers and faculty members
- The Python Software Foundation
- The Tkinter and MySQL communities for their documentation and open-source resources
---
## ⭐ Support the Project

If you found this project useful or interesting, please consider giving it a **⭐ Star** on GitHub.

Your support helps others discover this project and encourages us to continue improving it. Thank you for checking out our work!

---

