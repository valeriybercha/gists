# INSTALL FLASK ON UBUNTU LINUX SYSTEM

1. Ubuntu 18.04 ships with Python installed by default. To check if Python is installed on the system run the following command in the terminal:
```python3 --version```
The Python version should be displayed.
2. Python virtual environment package should be installed. To installed it use the command: ```sudo apt install python3-venv```
3. Creating a virtual environment.
* Create a new project directory: ```mkdir flask_app```
* Navigate to the directory: ```cd flask_app```
* In the project directory the virtual envionment should be created: ``` python3 -m venv venv```
4. Activate the virtual environment with the command: ```source bin/activate```
5. Install Flask: ```pip install Flask```
6. To check if Flask was installed on the sytem type the following command: ```python -m flask --version``` Flask and Python versions should be displayed
7. Create the simpliest 'Hello World' program in Flask:
```
from flask import Flask
app = Flask(__name__)

@ app.route('/')
def hello_world():
    return "Hello, World!"
```
8. Launching the development server:
* Command: ```export FLASK_APP=hello.py```
* Command: ```flask run```
The ```http://127.0.01:5000``` server address should be displayed. Open it in the web browser and the message "Hello, World!" sould be displayed on the screen.
* Use ```deactivate``` command to stop the server.
