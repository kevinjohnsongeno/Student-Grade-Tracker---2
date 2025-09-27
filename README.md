#  GradeTracker Database

**GradeTracker** is a basic academic tracking system designed to store and manage:

- Student records
- Subject details
- Login credentials
- Marks and grading information

This README outlines how to initialize the database and describes the purpose of each SQL operation used in the setup.

---

##  Database: `gradetracker`

```sql
USE gradetracker;
##  SQL Commands Used in This Project

This project makes use of several fundamental SQL commands that enable interaction with the database. Below is an overview of each command with explanations and relevant examples from the GradeTracker project:

### 1. `USE`

- **Purpose:** Selects the database to perform subsequent operations.
- **Example:**
    ```sql
    USE gradetracker;
    ```

### 2. `INSERT INTO`

- **Purpose:** Adds new rows (records) to a table.
- **Example:** Inserting student records:
    ```sql
    INSERT INTO students(student_name, batch, username) 
    VALUES ("Kevin Johnson Geno", "E", "kevin@CSE");
    ```
- **Used for:** Populating `students`, `subjectdetails`, `studentlogin`, `adminlogin`, and `student_marks` tables.

### 3. `UPDATE`

- **Purpose:** Modifies existing data in a table.
- **Example:** Updating a student's username:
    ```sql
    UPDATE students 
    SET username = "albin@cse"
    WHERE student_id = 2;
    ```
- **Used for:** Correcting or changing records such as usernames and subject credits.

### 4. `DELETE`

- **Purpose:** Removes records from a table.
- **Example:** Deleting a student record:
    ```sql
    DELETE FROM students
    WHERE student_id = 5;
    ```
- **Used for:** Removing student records, their marks, or admin accounts as needed.

---

### Summary

By mastering these commands, you can:

- Select which database to work with (`USE`)
- Add new data (`INSERT INTO`)
- Update existing data (`UPDATE`)
- Remove unwanted data (`DELETE`)

These form the backbone of managing relational databases efficiently and are essential skills for working with any SQL-based system.

---

