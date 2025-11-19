

1. Open a MySQL client (e.g., MySQL Workbench or the MySQL command-line client).

2. To list all databases, run the following command:

   ```sql
   SHOW DATABASES;
   ```

3. Create a new database named "student" if it doesn't already exist:

   ```sql
   CREATE DATABASE student;
   ```

4. Switch to the "student" database:

   ```sql
   USE student;
   ```

5. Verify that you're in the "student" database:

   ```sql
   SELECT DATABASE();
   ```

6. Create a table named "students" to store student records. The table structure should match the fields you have in your Java application (name, ID, grade, date of birth, gender, contact, and email). Here's an example table structure:

   ```sql
   CREATE TABLE students (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(255),
       student_id VARCHAR(255) UNIQUE,
       grade VARCHAR(255),
       date_of_birth DATE,
       gender VARCHAR(10),
       contact VARCHAR(20),
       email VARCHAR(255)
   );
   ```

7. You can view the table structure with:

   ```sql
   DESCRIBE students;
   ```

8. Now you have the "student" database and the "students" table ready to use with your Java application.



## Usage

1. Launch the application.

2. Enter student details, such as name, ID, grade, date of birth, gender, contact, and email.

3. Click the "Add Student" button to add a student record.

4. Use the "Reset" button to clear the input fields.

5. Select a record in the table and click the "Delete Record" button to remove it.

6. Use the "Search by ID" field to search for a student by ID.
