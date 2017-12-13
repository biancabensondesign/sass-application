# blog_application
NYCDA project to assimilate all of the skills covered in the course, e.g Sequelize, RESTful routing, etc.

REQUIREMENTS: 
Sequelize
Restful routing
Connection string read from environment variables

PROJECT SPECIFICATION 
Create a blogging application that allows users to do the following:
- register an account X 
- login X 
- logout X
Once logged in, a user should be able to: 
- create a post X 
- view a list of their own posts X 
- view a list of everyone's posts X 
- view a specific post X, including the comments people have made about it 
- leave a comment on a post X

TABLE RELATIONSHIPS

User.hasMany(Blogpost)
User.hasMany(Comment)
Blogpost.belongsTo(User)
Blogpost.hasMany(Comment)
Comment.belongsTo(User)
Comment.belongsTo(Blogpost

TABLES						
Blogposts	id	title	body	createdAt	updatedAt	userId
Users id	username	email	password		
Comments	id	body	createdAt	updatedAt	userId	

Where	        Type of request
Landing page	app.get
Home	        app.get
Log in	      app.post
Register	    app.post
Profile	      app.get
Create post	  app.get 
Show new post	app.get 
Your posts	  app.get 
Blogfeed	    app.get
Blogfeed	    app.get
Comment	      app.post
View single post with comment	app.get
Bcrypt	      N/A
Data Validation	
Logout	      app.get
Listen on port app.listen
						

