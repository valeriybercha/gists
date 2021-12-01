# Create and add Flask secret key configuration

- Open the flask project file and add the configuration for the secret key: ```app.config['SECRET_KEY'] = 'your_secret_key'```
- Generate a secret key with Python and 'os' module:
	- start Python in terminal ```python3```
	- import 'os' module ```import os```
	- create a random hex string ```os.uramdom(12).hex()```
	- copy and paste the resulted random string in the Flask project secret key
