# ST10475290poe3
# ChatApplication
## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [File Structure](#file-structure)
- [License](#license)

## Overview
QuickChat is a Java-based console messaging application that enables users to securely register, send messages, and track message history. The application features robust input validation and message management capabilities.

## Features
- *User Authentication*
  - Secure registration with password complexity requirements
  - Username validation (3-15 alphanumeric characters)
  - Phone number validation (South African format)
  
- *Messaging System*
  - Send messages with 250-character limit
  - Message status tracking (sent/received/stored)
  - Unique message ID generation
  - Message hashing for verification

- *Reporting*
  - View recently sent messages
  - Generate message statistics reports
  - Track total message count

## Requirements
- Java JDK 11 or later
- Maven (for building)

## Installation
1. Clone the repository:
bash
git clone https://github.com/yourusername/quickchat.git
cd quickchat


2. Build the project:
bash
mvn clean package


## Usage
Run the application:
bash
java -jar target/quickchat.jar


*Menu Options:*
1. Register new account
2. Login with existing credentials
3. Send messages
4. View message history
5. Generate reports
6. Exit

## Testing
Run unit tests:
bash
mvn test


## File Structure

quickchat/
├── src/
│   ├── main/java/
│   │   ├── ChatApplication.java    # Main application
│   │   ├── User.java               # User model
│   │   └── Message.java            # Message model
│   └── test/java/
│       └── ChatApplicationTest.java # Unit tests
├── target/                        # Build output
├── stored_messages.json           # Persisted messages
└── pom.xml                        # Maven config


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
