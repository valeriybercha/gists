# Create and test Flask SQLite project database with SQLAlchemy

### Pre-requisites:
- Flask application 'app.py' should be already created.

1. Install Flask SQLAlchemy package: ```pip install flask-sqlalchemy```
2. Create the tables for the project:
```
from flask_sqlalchemy import SQLAlchemy

app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///site.db'

db = SQLAlchemy(app)

class User(db.Model):
	id = db.Column(db.Integer, primary_key=True)
	username = db.Column(db.String(20), unique=True, nullable=False)
	email = db.Column(db.String(120), unique=True, nullable=False)
	image_file = db.Column(db.String(20), nullable=False, default='default.jpg')
	password = db.Column(db.String(60), nullable=False)
	post = db.relationship('Post', backref='author', lazy=True)
	
	def __repr__(self):
		return f"User('{self.username}', '{self.email}', '{self.image_file}')"


class Post(db.Model):
	id = db.Column(db.Integer, primary_key=True)
	title = db.Column(db.String(100), nullable=False)
	date_posted = db.Column(db.DateTime, nullable=False, default=datetime.utcnow)
	content = db.Column(db.Text, nullable=False)
		user_id = db.Column(db.Integer, db.ForeignKey('user.id'), nullable=False)
	
	def __repr__(self):
		return f"User('{self.title}', '{self.date_posted}')"
```
3. Open ```python``` in terminal in the virtual environment
4. From application 'app' import 'db', 'User' and 'Post':
	- ```from flaskblog import db```
	- ```from flaskblog import User, Post```
5. Create a database with the command: ```db.create_all()``` "site.db" file shoulf be created in the project directory
6. Create a new user:
```
user_1 = User(username="John", email="JohnDoe@company.com", password="password")
db.session.add(user_1)
db.session.commit()
```
7. Verify if users were added to database (will display all the users): ```User.query.all()```
8. Verify the first user added: ```User.query.first()```
9. Filter users added by name (case sensitive): ```User.query.filter_by(username="John").all()```
10. Additional queries:
	- Set up a variable "user" ```user = User.query.first()```
	- display user id: ```user.id```
	- display the user by id: ```User.query.get(1)```
	- display users posts: ```user.post```
11. Create a new post:
```
post_1 = Post(title="First blog post", content="First post content", user_id=user.id)
db.session.add(post_1)
db.session.commit()
```
12. Additional queries:
	- ```user = User.query.get(1)```	
	- ```for post in user.post: print(post)```
	- ```post.author```
13. Delete all data: ```db.drop_all()```
14. Create a new blank database: ```db.create_all()```
