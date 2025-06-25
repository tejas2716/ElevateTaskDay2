
Tejas Tukaram Sathe
sathetejas111@gmail.com
Pune, Maharashtra, India


# 🎓 Student Record Management System (Java)

This is a simple **console-based Java application** for managing student records using object-oriented programming and custom exception handling. It allows users to perform **CRUD operations** (Create, Read, Update, Delete) on student data, with input validation and proper user prompts.

---

#Features

- Add Student with validation (no negative marks)
- View all students
- Update student details by ID
- Delete student by ID
- Input validation using custom exception `InvalidMarks`
- Reusable menu-driven loop
- Graceful error handling (`InputMismatchException`, `InvalidMarks`)

#Project Structure

com.elevate_Internship_day_2/
├── StudentManagementSystem.java # Main class with menu and logic
├── Student # Student class with display method and validation
└── InvalidMarks # Custom exception class

#Technologies Used

- Java SE (Standard Edition)
- OOP (Object-Oriented Programming)
- Exception Handling
- Collections API (`ArrayList`)
- CLI (Command Line Interface)

#How It Works

#Step-by-Step Execution

1. Program starts from `main()` and calls `menu()`.
2. User is presented with 5 options:
    - 1 Add Student
    - 2 View Students
    - 3 Update Student
    - 4 Delete Student
    - 5 Exit
3. User chooses an option by entering a number.
4. Input is taken using `Scanner`.
5. Validation ensures:
    - ID and marks are numeric.
    - Marks are greater than 0 (else `InvalidMarks` is thrown).
6. Based on the choice, the corresponding method is executed.
7. If an exception is encountered, it is caught and a proper message is shown.


#Sample Console Run

===== Student Record Management System =====

Add Student

View Students

Update Student

Delete Student

Exit
Choose an option: 1
Enter ID: 101
Enter Name: Tejas
Enter Marks: -5
Enter Valid Marks...!

===== Student Record Management System =====

Add Student

View Students
Choose an option: 1
Enter ID: 101
Enter Name: Tejas
Enter Marks: 85
Student added successfully!

#Custom Exception: `InvalidMarks`

This exception is used to ensure that students cannot be added or updated with marks ≤ 0.

---java
class InvalidMarks extends Exception {
    // No logic required. It just signals invalid data
}

#Input Validation
Condition	Handled by
Non-numeric input	InputMismatchException
Marks ≤ 0	InvalidMarks (custom exception)

#Requirements
-Java JDK 8 or higher
-IDE (IntelliJ, Eclipse, VS Code) or terminal

#How to Run
-Clone or download the project folder.
-Open the folder in your IDE.
-Compile and run StudentManagementSystem.java.

#Future Improvements
-File handling to store records persistently.
-GUI version using JavaFX or Swing.
-Sorting and filtering functionality.
-Search by name or range of marks.

