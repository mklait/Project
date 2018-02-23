I created a sample application where users can post microposts and follow users using Ruby on Rails. Here are a few points about this application:
- Controllers: Users controller, Sessions controller, Microposts controller,  and Relationship controllers. 
- In each of these controllers, I used the CRUD HTTP operations for GET, POST, PUT, DELETE by the RESTful API resource for showing, creating, updating or deleting users, microposts, and relationships with users. 
- Users, microposts, and relationships have corresponding models which detail the association between models as well as validation rules. For example users have many microposts, many followers, and many relationships; microposts belong to a user, and users can follow other users and be followed by other users. 
-  I set up an authentication system so that users can sign up and then sign in (sessions). Instead of using devise, I practiced implementing Rails authentication. The user model includes the logic for validating users and ensuring safety of passwords. The sessions controller creates new sessions when users log in and destroys the sessions when logged out. 
- Each of the controllers has corresponding views. In the users views (edit, index, new, show), I remove duplicated code by refactoring the new.html.erb and edit.html.erb views to instead use the partial I created(_form.html.erb). 
- I wrote automated tests to automate the testing of the sign up form, the login in functionality, and to test for successful and unsuccessful edits of users. 
- I used bootstrap (gem for ruby) to style the front-end, most notably the navbar on the home page and sign up form (custom.scss)
