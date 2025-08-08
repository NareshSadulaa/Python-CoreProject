## 🎓 Exam Management System (Python + MySQL)

This is a **console-based Exam Management System** built using **Python** and **MySQL**.
It allows **Admins**, **Students**, and **College Officials** to manage and view examination-related information, including **exam centers**, **seat numbers**, **college details**, and **student registrations**.

---

### ✨ Features

#### 👨‍💼 Admin

* Login with email and password.
* View and remove registered colleges.
* View and remove students.
* Manage exam centers:

  * Display all centers.
  * Assign students to centers with seat numbers.
  * Remove students from exam centers.

#### 🎓 Student

* Register with name, email, and password.
* Login to:

  * Check seat number.
  * Check exam center.

#### 🏫 College Official

* Register a college with name, email, password, and available seats.
* Login to:

  * View students allotted to the college for exams.
  * Check remaining exam seats.

#### 📍 Exam Center Management

* Random assignment of students to colleges for examination.
* Auto-generated seat numbers.
* View and delete student exam center data.

---

### 🛠️ Technologies Used

* **Python** – Core application logic.
* **MySQL** – Database for storing records.
* **mysql-connector-python** – Python-MySQL connectivity.
* **Random Module** – For random seat number and center allocation.

---

### 📂 Database Structure

**Database:** `exam_management`
**Tables:**

* `admin_table` – Stores admin credentials.
* `student_table` – Stores student details.
* `college_table` – Stores college details and seat availability.
* `exam_center` – Stores assigned exam center and seat numbers.

---

### 🚀 How to Run

1. Install dependencies:

   ```bash
   pip install mysql-connector-python
   ```
2. Create MySQL database and tables:

   ```sql
   CREATE DATABASE exam_management;
   ```

   *(Tables are auto-created when running the script if they don't exist.)*
3. Update MySQL credentials in the code if needed.
4. Run the application:

   ```bash
   python exam_management.py
   ```
