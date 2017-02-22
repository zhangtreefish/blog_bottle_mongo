#blog_bottle_mongo
This is a blog application project from MongoUniversity using MongoDB3.4,
Python 2.7 and Bottle, the one-file Python microframework.
1. Install [MongoDB](https://www.mongodb.com/download-center#community)
2. git clone this project
3. cd into the directory where blog.py is.
4. start mongod instance by:
```sh
mkdir data
mongod --dbpath data
```
5. start the blog application by:
```
pip install pymongo
pip install bottle
python blog.py
```
6. Visit http://localhost:8082/ to post at the blog
7. start `mongo` shell to connect to the database; once inside:
```
show dbs # get admin, blog, local
use blog
show collections # get posts, sessions, users
db.users.find()
db.posts.find().pretty()
db.sessions.find()
```
