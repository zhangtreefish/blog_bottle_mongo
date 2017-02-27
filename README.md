#blog_bottle_mongo
This is a blog application project from MongoUniversity using MongoDB3.4,
Python 2.7 and Bottle 0.12.13, the one-file micro web-framework for Python.

Install [MongoDB](https://www.mongodb.com/download-center#community);

git clone this project;

cd into the directory where blog.py is.

start mongod instance by:
```sh
mkdir data
mongod --dbpath data
```

populate 'posts' data with:
```
mongoimport -d blog -c posts < posts.json
```

start the blog application by:
```
pip install pymongo
pip install bottle
python blog.py
```
Visit http://localhost:8082/ to post at the blog;

start `mongo` shell to connect to the database; once inside:
```
show dbs # get admin, blog, local
use blog
show collections # get posts, sessions, users
db.users.find()
db.posts.find().pretty()
db.sessions.find()
```
