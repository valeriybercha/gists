# Hashing password in Flask before adding it to the database

- Import the library ```from werkzeug.security import generate_password_hash, check_password_hash```
- Create a variable ```psw``` with the following value for password ```12345```: ```pass = generate_password_hash("12345")```
- Print the ```psw``` variable: ```print(psw)``` Hashed password should be displayed
- Verify hashed password: ```check_password_hash(psw, "12345")```
