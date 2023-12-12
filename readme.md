# Libsec Ashesi Library Management System

## Project Overview

This Library Management System is a web application designed to efficiently manage and monitor the borrowing of books from a school library. The system incorporates RFID technology, allowing each book to be uniquely identified and tracked. The primary functionalities include librarian book search, book checkout, and overall library book management.

## Software Functionality

### Librarian Book Search:
- Librarians can search for books by name or RFID value.
- The system provides real-time search results, facilitating quick book identification.

### Librarian Checkout:
- Librarians can initiate book checkout for students.
- The checkout page allows librarians to enter student email, student ID, and borrow duration.
- Upon approval, the system updates the book's approval status and sets the return date.

### Library Book Management:
- Librarians can add new books with RFID and book names.
- The system displays a list of all books with approval and buzzer status.
- Librarians can edit book details, including approval and buzzer status.
- Books can be deleted from the system.

### RFID Security:
- The system integrates an ESP32 with an RFID sensor at the library gate.
- An alarm is triggered if a book with a false approval status exits without passing through the librarian's checkout process.

## Technology & Justification

### Technologies Used:
- **HTML5 and CSS:** Used for creating the web-based user interface.
- **JavaScript:** Employed for client-side scripting and Firebase Realtime Database interactions.
- **Firebase:** Integrated for real-time database storage and retrieval, enabling seamless data management.
- **ESP32 and RFID Sensor:** Implemented for security at the library gate, ensuring RFID verification.

### Justification:
- **Web Application:** Chosen for accessibility and ease of use. Web applications can be accessed from various devices with a browser, making it convenient for librarians.
- **Firebase Realtime Database:** Selected for its real-time syncing capability, providing instant updates to librarians and ensuring data consistency.
- **ESP32 and RFID:** Utilized for enhanced security. RFID technology allows for efficient book tracking, and the ESP32 with Firebase integration ensures a real-time check against the database.
