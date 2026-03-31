# CampusCore (formerly CCRM)

A robust Java-based academic management system designed specifically for managing student records, course enrollments, and academic performance tracking. 

## 🌟 Key Features

*   **Student Management**: Add, view, search, and update comprehensive student profiles (ID, registration number, department).
*   **Course Management**: Create and oversee courses across diverse departments (Computer Science, Electrical Engineering, etc.) with credit tracking.
*   **Enrollment System**: Enroll/unenroll students while strictly enforcing institutional rules (e.g., maximum 18 credits per semester, no duplicates).
*   **Grade Management**: Grade recording and real-time GPA calculations based on standard alphabetical grades (S, A, B, C, D, E, F).
*   **Data Import/Export**: Efficiently process bulk records using CSV files for students and courses. Includes system backups.

## 🛠️ Technical Details

*   **Language**: Java 8+
*   **Architecture**: Object-Oriented Design (OOD) enhanced with Service Layer and Domain-Driven Design principles.
*   **Design Patterns**: Builder Pattern, Singleton Pattern, Command Pattern.
*   **Key APIs Used**: File I/O (NIO.2), Stream API, Java Collections Framework.

## 🚀 Getting Started

### Prerequisites
*   Java Development Kit (JDK) 8 or higher.

### Running the Application
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Tim3-19/CampusCore.git
   cd CampusCore
   ```
2. **Compile the source code:**
   Ensure you compile all the source files inside the `src` directory into a `bin` directory, or use your preferred IDE (Eclipse/IntelliJ) which will do this for you.
3. **Execute:**
   Run the main class from the compiled `bin` directory, enabling assertions (recommended):
   ```bash
   java -cp bin -ea edu.ccrm.Main
   ```
   *Note: If data/backups aren't populating, ensure the application is run from the project root where these directories reside.*

## 📂 Project Structure

```text
CampusCore/
├── src/           # Application Source (Controllers, Domain Models, Services, I/O)
├── bin/           # Compiled Java classes
├── data/          # App data storage and persistent files
├── backups/       # Auto-generated backup files
└── test-data/     # CSV files for testing import capabilities
```

## 📜 Usage Operations

When you start the application, you'll be navigated to a main menu. You can:
- **Option 1**: Manage Students
- **Option 2**: Manage Courses
- **Option 3**: Manage Enrollments
- **Option 4**: Manage Grades
- **Option 5**: Import/Export Data (CSV format located in `test-data`)
- **Option 6**: Perform Backups
- **Option 7**: View Reports
