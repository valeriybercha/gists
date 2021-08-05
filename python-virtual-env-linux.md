# Python virtual environment setup on Linux

1. Install pip if it's not already installed on the machine
```sudo apt-et install python3-pip```

2. Create a virtual environment
- ```cd 'to project directory'```
- ```virtualenv venv```

3. Activate the environment
```source venv/bin/activate```

4. Add libraries and create requirements.txt file
- ```pip 'libraries to install'```
- ```pip freeze > requirements.txt``` (create the requirements.txt file enumerating the installed packages)

5. Deactivate the environment
```deactivate```
