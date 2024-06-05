
README for File Hider
Overview
File Hider is a Java application designed to securely hide files, ensuring privacy and confidentiality for users. It allows users to hide sensitive files and reveal them as needed, with authentication via OTP (One Time Password) sent to their email addresses.

Features
User Authentication: Users can log in or sign up using their email addresses and verify their identity via OTP sent to their email.
File Hiding: Once authenticated, users can hide files securely, ensuring they are not easily discoverable or accessible.
File Revealing: Users can reveal hidden files when needed, ensuring they have access to their hidden files whenever necessary.
Database Storage: User information and hidden file metadata are stored securely in a MySQL database.
Technologies Used
Java
JDBC (Java Database Connectivity)
JavaMail API for email communication
MySQL Database
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Ashusharma246/FileHider.git
cd filehider
Set up your MySQL database:

Create a new database in MySQL.
Run the provided SQL script (database.sql) to set up the necessary tables.
Configure the database connection in the project (src/main/resources/db.properties).
Configure email settings:

Update the email configuration in the project (src/main/resources/email.properties) with your SMTP server details.
Open the project in IntelliJ IDEA or your preferred IDE.

Build the project using Maven:

bash
Copy code
mvn clean install
Run the Java application from your IDE or using Maven:

bash
Copy code
mvn exec:java -Dexec.mainClass="com.example.views.Welcome"
Usage
Launch the application.

Choose to log in if you have an existing account or sign up if you're a new user.

Follow the prompts to authenticate via OTP sent to your email address.

Once authenticated:

To hide files, provide their paths.
To reveal hidden files, select the files from the list of hidden files.
Future Enhancements
Implement file encryption for added security.
Enhance the user interface for better usability.
Introduce multi-factor authentication for enhanced security.
Add a password recovery feature to assist users who forget their passwords.
Improve error handling and logging to better diagnose and address issues.
Support for multiple file hiding and revealing in batch mode.
Contributing
Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.

Fork the repository.

Create your feature branch:

bash
Copy code
git checkout -b feature/your-feature
Commit your changes:

bash
Copy code
git commit -am 'Add some feature'
Push to the branch:

bash
Copy code
git push origin feature/your-feature
Create a new Pull Request.
