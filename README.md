# Design Patterns

 ## First Design Pattern (MVC)
 
  The whole appliaction is based on (MVC) design pattern so the application contains three folders (Models, Views, Controllers)
 
 ## Second Design Pattern (Singletone)
 
  This design pattern is used to create only one object from the class
  I used this design pattern in (config.php) in order to get only one object from Database connection object
 
 ## Third Design Pattern (Strategy)
 
  This design is used to allow you to select function during runtime
  This mean that each subclass implements parent class and implement function that in parent class as needed with different implementation
  I used this design pattern in (Users.php and userController.php) to make two methods for admin layer login { can login with username and    password or login with email and password }
 
 
# Socail Media API

 In this project i used google plus api in order to login to system and be able to make comment on advertisements
 
 
# Database structure

  The database is called yellow and the sql file is in the repository and called (yellow.zip)
  The database consist of three tables
  
  ## First table for advertisements (ads)
   this table consist of
    (id) which is auto increment
    (image) name of image
    (description) description of advertisement
    
  ## Second table for users (users)
   this table consist of
   (id) which is auto increment
   (name) name of user
   (email) email of user
   (password) password of user
   (type) type for user role (0 =>'means he is admin', 1=>'means he is editor', 2=>'means he is user')
  
  ## Third table for comments (comments)
   this table consist of
   (id) which is auto increment
   (comment) subject of comment
   (created_at) the time in which the comment approved
   (status) the status of comment (0 => 'means not approved' , 1 => 'means approved')
   (user_id) foreign key with the id that exist in (users) table
   (ads_id) foreign key with the id that exist in (ads) table
   

 
