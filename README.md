# Web Application - Part 1

## Project Description

This project is all about creating an API for users with methods to CREATE, LOGIN, GET_DETAILS, UPDATE_DETAILS, LIST_ALL_USERS, GET_A_USER_BY_ID and DELETE (CRUD methods). This homework is a part of the class IS 601 of Fall 2019.

## Problem Statement
For this assignment you need to follow this tutorial to create the application.

[https://www.codementor.io/olawalealadeusi896/restful-api-with-python-flask-framework-and-postgres-db-part-1-kbrwbygx5](https://www.codementor.io/olawalealadeusi896/restful-api-with-python-flask-framework-and-postgres-db-part-1-kbrwbygx5) 

Upload it to Github and submit a link to the repo branch called "part1"

## Output
I have created the API to supported the required CRUD operations and the images of the same are as follows:

### CREATE:

The objective of this section is to create a user. We can see in the image that an user with the email id "kaustav@kaustav.com" has been created and the jwt token has been returned:


![Post Successful](/blog_api/images/Kaustav_Set/1.Create_User_Successful.png)

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