# Python virtual environment setup on Linux

1. Create a virtual environment
- cd 'to project directory'
- virtualenv venv

2. Activate the environment
- source venv/bin/activate

3. Add libraries and create requirements.txt file
- pip 'libraries to install'
- pip freeze > requirements.txt (create the requirements.txt file enumerating the installed packages)

4. Deactivate the environment
- deactivate
