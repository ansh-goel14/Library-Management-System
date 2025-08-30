# Library Management System (LMS)

A comprehensive Java-based Library Management System built with Swing GUI and MySQL database integration for managing library operations including book inventory, member management, and transaction tracking.

## 📋 Project Overview

This Library Management System is a desktop application designed to automate library operations. It provides a user-friendly interface for librarians to manage books, members, and transactions efficiently.

## 🚀 Features

- **Member Management**
  - Add, update, and delete library members
  - Track membership dates and expiry
  - Store complete member contact information

- **Book Management**
  - Comprehensive book catalog with details (Title, Author, Subject, Price)
  - Track book availability status
  - Manage book inventory

- **Transaction Management**
  - Issue and return books
  - Track transaction history
  - Manage due dates and returns

- **Publisher Information**
  - Maintain publisher details
  - Link books with their publishers

## 🛠️ Technology Stack

- **Language**: Java
- **GUI Framework**: Java Swing
- **Database**: MySQL
- **Date Picker**: JCalendar 1.4
- **Build Tool**: Apache Ant (NetBeans project)

## 📁 Project Structure

```
Library-Management-System/
├── src/                    # Source code and resources
├── build/                  # Compiled classes
├── nbproject/             # NetBeans project files
├── build.xml              # Ant build configuration
├── jcalendar-1.4.jar     # JCalendar library
├── Final Code_.txt        # Database schema and sample data
├── manifest.mf           # JAR manifest file
└── README.md             # Project documentation
```

## 🗄️ Database Schema

The system uses a MySQL database named `lms` with four main tables:

### Tables:
1. **MEMBER** - Store member information (ID, name, contact, address, membership details)
2. **BOOKS** - Book catalog (ID, title, author, subject, price, availability)
3. **TRANSACTION** - Track book issues/returns (transaction ID, book ID, member ID, dates)
4. **PUBLISHER** - Publisher information (ID, name, contact, address)

### Key Features:
- Foreign key relationships between tables
- Cascade operations for data integrity
- Sample data included for testing

## 🚀 Getting Started

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- MySQL Server
- NetBeans IDE (recommended) or any Java IDE

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Library-Management-System
   ```

2. **Set up the database**
   - Install and start MySQL server
   - Execute the SQL commands from [`Final Code_.txt`](Final Code_.txt) to create the database and tables

3. **Configure database connection**
   - Update database connection parameters in your Java code
   - Ensure MySQL JDBC driver is in the classpath

4. **Build the project**
   ```bash
   # Using Ant (if NetBeans)
   ant clean
   ant build
   
   # Or compile directly
   javac -cp "jcalendar-1.4.jar:." src/*.java
   ```

5. **Run the application**
   ```bash
   java -cp "build/classes:jcalendar-1.4.jar" MainClass
   ```

## 📊 Sample Data

The system comes pre-loaded with:
- 23 sample members
- 23 sample books across various subjects (Physics, Chemistry, Mathematics, English, etc.)
- 23 sample transactions
- 22 publisher records

## 🔧 Configuration

- **Database Configuration**: Update connection strings in the Java source files
- **UI Customization**: Modify Swing components as needed
- **Date Format**: Configured to use JCalendar for date selection

## 📝 License

This project is licensed under the MIT License - see the [`license`](license) file for details.

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

For support and questions, please open an issue in the project repository.

## 🎯 Future Enhancements

- Web-based interface
- Advanced search functionality
- Report generation
- Fine management system
- Book reservation system
- Multi-library support

---
