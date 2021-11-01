# Python virtual environment setup on Linux

1. Verify if Python and 'pip' are installed on the machine: ```python --version```. If not install:
	- Python ```sudo apt install python3```
	- 'pip': ```sudo apt install python3-pip```

2. Install virtual environment package:
	- 'venv' virtual environment: ```sudo apt install python3-venv```
	- 'virtuelenv' virtual environment: ```sudo apt install python3-virtualenv```

3. Navigate to project directory ```cd python-project``` and create virtual environment:
	- For 'venv' virtual environment: ```python3 -m venv venv```
	- For 'virtualenv' virtual environment: ```virtualenv venv```

4. Activate the environment: ```source venv/bin/activate```

5. Add libraries and create requirements.txt file
	- ```pip 'libraries to install'```
	- ```pip freeze > requirements.txt``` (create the requirements.txt file enumerating the installed packages)

6. Deactivate the environment: ```deactivate```
