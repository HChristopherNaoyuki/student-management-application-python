# Student Management System

This is a simple console-based Student Management System that allows users to add, search, delete, and view student records. It is implemented in Python using object-oriented programming principles. The application supports the following functionalities:

- **Capture a New Student**: Allows you to input and save a new student's information (ID, name, age, email, course).
- **Search for a Student**: Lets you search for a student by their ID and display their details.
- **Delete a Student**: Allows you to delete a student from the records by providing their ID.
- **Print Student Report**: Displays all the saved student records.
- **Exit the Application**: Exits the application with a goodbye message.

## Features

- Add new students with detailed information.
- Search for students by their student ID.
- Delete student records.
- Display a report of all students.
- Input validation for age (only allows ages 16 and above).
- User-friendly console interface for navigation and interaction.

## Installation

To run this application, you'll need to have Python installed on your system. The program uses basic Python features, so there are no external dependencies.

### Steps to Run the Application

1. Ensure Python is installed on your machine.
2. Copy the code into a Python file, e.g., `student_management.py`.
3. Open a terminal or command prompt and navigate to the directory containing the file.
4. Run the following command:

   ```bash
   python student_management.py
   ```

5. The program will display the menu where you can select different options to interact with the system.

## Application Workflow

1. **Launch the Application**: 
   - When you first run the program, you will be asked whether to launch the menu or exit the application.
   
2. **Menu Options**:
   - **Capture a New Student**: You will be prompted to enter the student's ID, name, age, email, and course.
   - **Search for a Student**: You can search for a student by entering their ID. If found, their details will be displayed.
   - **Delete a Student**: Enter the student's ID to delete their record from the system.
   - **Print Student Report**: This will display a report showing all the students currently stored in the system.
   - **Exit the Application**: Exits the program with a goodbye message.

3. **Student Records**: 
   - All student records are stored in memory within the application and are lost when the program exits. This can be extended by adding persistent storage like a database or file system.

## Example Usage

1. **Launch the Program**:
   - Enter (1) to launch the menu.

2. **Capture a New Student**:
   - Select (1) to capture a new student.
   - Enter the required details such as student ID, name, age, email, and course.

3. **Search for a Student**:
   - Select (2) to search for a student.
   - Enter the student ID you wish to search for.
   - If the student exists, their details will be displayed.

4. **Delete a Student**:
   - Select (3) to delete a student.
   - Enter the student ID and confirm if you want to delete the record.

5. **Print Student Report**:
   - Select (4) to print a report of all students.
   
6. **Exit the Application**:
   - Select (5) to exit the program.

## Example (Menu):
```text
Please select one of the following menu items:
(1) Capture a new student.
(2) Search for a student.
(3) Delete a student.
(4) Print student report.
(5) Exit Application.
```

## Code Structure

### `Student` Class
The `Student` class contains the following:
- **Attributes**: `student_id`, `name`, `age`, `email`, `course`.
- **Static Methods**:
  - `save_student()`: Adds a new student to the system.
  - `search_student()`: Searches for a student by ID.
  - `delete_student()`: Deletes a student by ID.
  - `student_report()`: Prints a report of all students.
  - `exit_student_application()`: Exits the application.

### `StudentManagementApplication` Class
The `StudentManagementApplication` class manages the application menu and user input. It includes:
- **Menu Display**: `show_menu()`.
- **Student Capture**: `capture_student()`.
- **Student Search**: `search_student()`.
- **Student Deletion**: `delete_student()`.
- **Application Control**: `main()` to run the application.

## Example Code

```python
# Main method to run the application
if __name__ == "__main__":
    StudentManagementApplication.main()
```

## Limitations

- The program currently stores student data only in memory (i.e., once the application is closed, all data is lost).
- No persistent storage mechanism (e.g., database or file system) is implemented.
- The system does not support user authentication or role-based access.

## Future Enhancements

- Integrate a database (e.g., SQLite, MySQL) to persist student records.
- Add more features such as updating student records.
- Implement user authentication for secure access to the system.
- Create a graphical user interface (GUI) for better user experience.

---
