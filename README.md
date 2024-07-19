## Overview

The Clinic Management System is a console-based Java application designed to help healthcare providers manage patients, appointments, and medical records efficiently. This application demonstrates proficiency in Core Java, MySQL, and JDBC.


## Features

- **Patient Management**
  - Add a new patient
  - View patient details
  - Update patient information
  - Delete an patient

- **Appointment Management**
  - Schedule a new appointment
  - View appointment details
  - Update appointment information
  - Cancel an appointment

- **Medical Record Management**
  - Add a new medical record
  - View medical record details
  - Update medical record information
  - Delete a medical record


## Prerequisites

- JDK 8 or higher
- MySQL 5.7 or higher
- Eclipse IDE (optional, but recommended for development)
- MySQL JDBC Driver


## Installation

### Step 1: Clone or Download the Repository

1. Clone the repository using Git (if you have Git installed):
   ```bash
   git clone https://github.com/yourusername/clinic-management-system.git
   ```
or

2. Download the ZIP file from GitHub and extract it:
     - Go to the GitHub repository.
     - Click the green `Code` button.
     - Select `Download ZIP`.
     - Extract the ZIP file to your local machine.

### Step 2: You can either create your own database or use the schema already provided.

### Step 3: Configure the Project in Eclipse

1. Open Eclipse IDE.

2. Import the project:
      - Go to `File` > `Import...`.
      - Select `General` > `Existing Projects into Workspace`.
      - Click `Next`.
      - Browse to the directory where you extracted the project.
      - Select the project and click Finish.

3. Add MySQL JDBC Driver to the build path:
      - Right-click on the project in Project Explorer.
      - Select `Build Path` > `Add External Archives...`.
      - Browse to the location of the MySQL JDBC Driver JAR file provided (or the one already present in the local system) and add it.

### Step 4: Build and Run the Project

1. Right-click the `src` folder or the main class file `Application.java` in the Project Explorer.

2. Select `Run As` > `Java Application`.


## Project Structure

```plaintext
ClinicManagementSystem
├── JRE System Library [JavaSE-21]
├── JRE System Library [JavaSE-22]
├── src
│   ├── app_data
│   │   ├── Application.java
│   │   ├── AppointmentDB.java
│   │   ├── MedicalRecordDB.java
│   │   └── PatientDB.java
│   ├── base_data
│   │   ├── Appointment.java
│   │   ├── MedicalRecord.java
│   │   └── Patient.java
│   ├── dao
│   │   ├── AppointmentDAO.java
│   │   ├── MedicalRecordDAO.java
│   │   └── PatientDAO.java
│   └── dbcon
│       ├── DBconnect.java
│       └── DBUtil.java
└── Referenced Libraries
    └── mysql-connector-j-9.0.0.jar
```

## Viewing Data in MySQL

### Using MySQL Command Line Interface

1. Open your terminal or command prompt.

2. Connect to your MySQL server:
```bash
mysql -u root -p
```

3. Switch to the `clinic` database:
```sql
USE clinic;
```

4. View data in the `Patient` table:
```sql
SELECT * FROM Patient;
```

5. View data in the `Appointment` table:
```sql
SELECT * FROM Appointment;
```

6. View data in the `MedicalRecord` table:
```sql
SELECT * FROM MedicalRecord;
```

### Using MySQL Workbench

1. Open MySQL Workbench.

2. Connect to your MySQL server.

3. Switch to the clinic database.

4. Use the SQL Editor to run queries like:
```sql
SELECT * FROM Patient;
```

```sql
SELECT * FROM Appointment;
```

```sql
SELECT * FROM MedicalRecord;
```
