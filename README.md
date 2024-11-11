# Student-Attendence-Management-system
Student Attendance Management System (Report) 

Python3 



Krishna Paul (12033028) 

Shariar Khan (12033913) 


Overview 

The Student Attendance Management System is designed to handle the registration of students and the recording of their attendance in a classroom setting. This application is developed using Python, with Tkinter for the graphical user interface (GUI) and Pandas for data management. ​The primary objective of the​ system ​is to provide​ instructors ​with an easy-to-use​ tool for tracking attendance while ensuring the protection of student data through secure access control and role-based authentication. 


The system’s functionality includes: 

Student registration 
Attendance marking 
Data storage and retrieval 
Secure login for instructors 
The system is built with maintainability in mind, following best practices in programming and ensuring the code is easy to update and test. 

 


System Design and Planning (15%) 

Conceptual Design 

The system supports two types of users: 

Students: Can register themselves in the system using their name. 
Instructors: Can log in using a password, mark attendance for students, and view attendance reports. 
The system is designed to be simple yet effective, allowing instructors to easily manage student attendance. The attendance data is securely stored and can be accessed or modified by authorized users only. 



Data Model 

The application uses CSV files to store student and attendance data: 

students.csv: Contains student IDs and names. 
attendance.csv: Tracks the attendance status (present/absent) for each student, along with the date. 
 

 

Here’s how the data is structured: 

 

The system uses Pandas to load, store, and manipulate data. If the CSV files do not exist, they are created automatically. 

 

Core Functionality (25%) 

Student Registration Mechanism 

The Student Registration feature allows students to register themselves by entering their name. A unique student ID is generated for each student. 

Here is the relevant code for the student registration process: 

The register_student function appends the new student to the students.csv file. 

 

 

Attendance Recording System 

Instructors can log in and mark attendance for students. They select a date, and then checkboxes are displayed for each registered student. The instructor can mark attendance by selecting the appropriate checkbox. 

Here’s the code for attendance marking: 

The mark_attendance function stores the attendance records in the attendance.csv file: 

Data Storage and Retrieval 

The system loads data using the load_data() function and saves it with save_data(). This ensures persistence across sessions. The attendance.csv and students.csv files are updated every time the attendance is marked or a student is registered. 

User Interface (UI) Development (15%) 

The system's interface is developed using Tkinter, making it accessible and easy to navigate. The UI features: 

A login screen for both students and instructors 
A student registration page 
An attendance marking page for instructors 
For example, the login page is created with the following code: 

Security and Privacy (10%) 

Data Privacy Measures 

Sensitive student data, such as attendance records, are stored securely in the system. Access to this data is restricted to authorized users only. Additionally, all login credentials (both admin and instructor) are validated before access to data is granted. 

Role-Based Access Control 

Access to features is determined by the role of the user: 

Students: Can only register and access their own information. 
Instructors: Can mark attendance, view student lists, and generate attendance reports. 
 

Documentation and Testing (20%) 

Documentation 

The code is well-documented with inline comments explaining the logic behind the different parts ​of the system. The​ user manual ​provides​ clear ​instructions​ for ​how to​ use the system, including registration, attendance marking, and generating reports. 

Unit Testing 

The system undergoes unit tests for key functions: 

Testing Student Registration: Verifies that student data is properly saved and retrieved. 
Testing Attendance Marking: Ensures that attendance is recorded accurately in the CSV file. 
Code Style 

The code adheres to PEP 8 style guidelines, ensuring consistency in naming conventions, indentation, and code structure. This facilitates readability and future maintenance. 

 

Requirements 

To successfully run the Student Attendance Management System, ensure that your development environment meets the following requirements: 

Software Requirements 

Python: The system is developed using Python 3.7+. You can download the latest version of Python from python.org. 
Tkinter: This is the default GUI library for Python and is required for the user interface. Tkinter comes pre-installed with Python, so you do not need to install it separately in most environments. However, you can verify or install it using: 
bash 
sudo apt-get install python3-tk    # For Ubuntu/Linux 
brew install python-tk             # For macOS (if not already installed) 
 
Pandas: This library is used for handling and manipulating CSV data. Install it using: 
bash 
pip install pandas 
 
Pillow: The Pillow library is used for image handling, which is required in your project. ​You can install it using:​ 
bash 
pip install pillow 
 
qrcode: This library is used to generate QR codes. You can install it via: 
bash 
pip install qrcode 
 
tkcalendar: This library is used for the calendar widget to allow instructors to select dates for attendance. Install it using: 
bash 
pip install tkcalendar 
 
Hardware Requirements 

Operating System: The system should run on any major operating system, including: 
​​Windows (7 or later)​ 
​​macOS (10.12 or later)​ 
​​Linux (Ubuntu​, Debian, Fedora, etc.) 
Memory: A minimum of 2 GB RAM is recommended for running the application smoothly. 
Storage: The application stores student and attendance data in CSV files. Ensure you have at least 50 MB of free disk space to store data and logs, which should be sufficient for small to medium-sized class data. 
Running the Project 

Clone or Download the Project Files: 
If you have a GitHub repository, you can clone it: 
 
bash 
​​git clone https://github.com/yourusername​/attendance-management.git 
 
Alternatively, download the ZIP file of the project and extract it to your desired directory. 
Navigate to the Project Directory: 
bash 
cd /path/to/attendance-management 
 
Run the Python Application: To start the application, run the following command: 
bash 
python3 attendance_management.py 
 
Optional - Create Virtual Environment: For managing dependencies in a controlled environment, you can ​create a virtual environment:​ 
bash 
python3 -​m venv​ venv 
source venv/bin/​activate      # On Windows​, use ​venv\Scripts​\activate 
pip install -r requirements.txt 
 
 

Contributions 

We welcome contributions from developers to improve and extend the system. Fork the repository, make changes, and submit a pull request. 

 

Developers 

The Student Attendance Management System was developed by krishna paul(12033028), shariar khan (12033913) 

For any inquiries or further information, please contact us via the project repository. 

Screenshot 

 

 

GitHub Link: 

Student-Attendence-System/Python_assignment final.py at main · Krishna12033/Student-Attendence-System 

https://github.com/shariar87/Student-Attendence-Management-system 

 

 
