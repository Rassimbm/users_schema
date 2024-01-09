Create 3 new users 
INSERT INTO users (first_name , last_name , email) VALUES ("Jesse" , "Pinkman" , "jesse.p@gmail.com"), ("Vitorio" , "Scaletta" ,
"vito.s@gmail.com") , ("Jin" , "Sakai" , "jin.s@gmail.com");

Retrieve all the users
SELECT * FROM users;

Retrieve the first user using their email address
SELECT email FROM users LIMIT 1;
SELECT * FROM users WHERE email = "jesse.p@gmail.com";

Retrieve the last user using their id
SELECT * FROM users ORDER BY id LIMIT 1;

Change the user with id=3 so their last name is Pancakes
UPDATE users SET last_name = "Pancakes" WHERE id = 3;

Delete the user with id=2 from the database
DELETE FROM users WHERE id = 2;

Get all the users, sorted by their first name
SELECT * FROM users ORDER BY first_name;

Get all the users, sorted by their first name in descending order
SELECT * FROM users ORDER BY first_name DESC;



