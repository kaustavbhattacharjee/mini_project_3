# Setting up Docker, Flask and SQLAlchemy

## Project Description

This project is all about setting up docker, flask and sqlalchemy as a part of the homework in class IS 601 of Fall 2019.

## Problem Statement
Complete this tutorial on getting Docker, Flask, Postgres and SQLalchemy working together:

[https://medium.com/@hmajid2301/implementing-sqlalchemy-with-docker-cb223a8296de](https://medium.com/@hmajid2301/implementing-sqlalchemy-with-docker-cb223a8296de) 

You can use this as the basis for the 3 part tutorial, since the tutorial doesn't cover getting Docker, Flask, and Postgres setup.

 

Submit a link to the repo on Github

## Output
We have used the following commands to insert,delete and edit data into the database and following are the images of the same:

**INSERT:**

```
curl -XPOST -H "Content-type: application/json" -d \
'{"name": "catty mcCatFace", "price": 5000, "breed": "bengal"}' \
'127.0.0.1:5000/add'
```

```
curl -XPOST -H "Content-type: application/json" -d \
'{"name": "catty kebby", "price": 6000, "breed": "American"}' \
'127.0.0.1:5000/add'
```

Data insertion is successful as per the following image.


![Post Successful](/images/post_successful.png)

**DISPLAY:**

```
curl -XGET -H "Content-type: application/json" \
'127.0.0.1:5000'
```

Data is displayed in the following image:


![Get Successful](/images/get_successful.png)


**REMOVE:**

```
curl -XDELETE -H "Content-type: application/json" \
'127.0.0.1:5000/remove/2'
```

Data removal is successful as per the following image.


![Remove Successful](/images/delete_successful.png)

**EDIT:**

```
curl -XPATCH -H "Content-type: application/json" -d \
'{"price": 7000}' \
'127.0.0.1:5000/edit/1'
```

Data editing is successful as per the following images.


![Edit Successful](/images/edit_successful.png)

![Edit Successful 2](/images/edit_successful2.png)