# Personal Data Project

## Overview

This project explores the handling and protection of personal data, focusing on how to secure Personally Identifiable Information (PII) effectively. By the end, you'll be able to explain key security concepts and implement basic protections around sensitive information.

## Learning Objectives

Upon completion of this project, you should be able to:

- **Identify Examples of Personally Identifiable Information (PII)**  
  Understand what constitutes PII, including common examples such as names, Social Security numbers, addresses, and other data that can be used to identify individuals.

- **Implement a Log Filter to Obfuscate PII Fields**  
  Develop logging practices that protect PII by filtering or masking sensitive fields in logs, ensuring that only non-sensitive information is recorded for security and compliance.

- **Encrypt and Validate Passwords**  
  Learn how to securely encrypt user passwords and verify the validity of password inputs using industry-standard methods, providing enhanced protection against unauthorized access.

- **Authenticate to a Database Using Environment Variables**  
  Implement a secure method for database authentication by using environment variables to store and access credentials, reducing the risk of exposing sensitive information within the code.

## Project Tasks

This project will cover practical steps, including:

1. **Identifying and Classifying PII**  
   Define and categorize data types that qualify as PII and understand the importance of securing each category.

2. **Log Filtering**  
   Set up a log filter to automatically detect and obfuscate PII within log messages.

3. **Password Encryption**  
   Use a hashing algorithm to securely encrypt passwords, ensuring they are stored in a non-readable format. Validate user input against the encrypted data.

4. **Database Authentication**  
   Configure your application to securely connect to a database using environment variables, ensuring database credentials are not hard-coded into the application.

## Instructions

1. **Install Dependencies**  
   Ensure all necessary libraries for encryption, logging, and database access are installed.

2. **Set Up Environment Variables**  
   Store sensitive information, such as database credentials, in environment variables. 

3. **Run and Test the Application**  
   Execute tests for log filtering, password encryption, and database authentication to confirm the security measures work as expected.

## Security Best Practices

- Always mask PII in logs to prevent accidental exposure.
- Never store plaintext passwords; always use encryption.
- Store database credentials and other sensitive configurations in environment variables, not in code.

By following these practices, you’ll be able to manage personal data securely and confidently.