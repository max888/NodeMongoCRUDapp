NodeMongoCRUDapp
================

This is a small app using MongoDB, NodeJS and Express to build a simple address book.



To run you will need to create a mongoDB on your local machine.

1.) Download MongoDB from http://mongodb.org/ 

2.) Wherever you download mongo to, get in that directory and run: mongod --dbpath c:\node\nodetest1\data

  You'll see the Mongo server start up.
  
  Once it says "[initandlisten] waiting for connections on port 27017", you're good. There's nothing more to do here; the server is running. 

3.) Now you need to open a second command prompt. Navigate again to your Mongo installation directory, and type: mongo

4.) In your client type:  db.usercollection.insert({ "username" : "testuser1", "email" : "testuser1@testdomain.com" })

  This creates collection called 'usercollection' and inserts the first dummy user. DB is now ready for more users.
  
5.) Back in another command line window in the nodetest1 directory, type: npm start

6.) app should be running on localhost:3000/newuser


Created with help from this tutorial: http://cwbuecheler.com/web/tutorials/2013/node-express-mongo/
