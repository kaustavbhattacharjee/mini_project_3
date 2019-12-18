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


![Create_User_Successful](/blog_api/images/Kaustav_Set/1.Create_User_Successful.png)

### READ:

The objective of this section is to read the user data. This is achieved in the following ways:

**Login:**

Here the user logs in with the email id and the password and an unique jwt token is returned which is used for other user activities.

![Login_User_Successful](/blog_api/images/Kaustav_Set/2.Login_User_Successful.png)


**Read User Data:**

Here the user's details like the email id, name, id, password(hashed), date created and date modified are returned, provided the api-token generated in the last step is passed on.

![Get_User_Successful](/blog_api/images/Kaustav_Set/3.Get_User_Successful.png)

**Read All User Data:**

Here the details of all the users are returned, provided proper api-token is passed on.

![List_All_Users_Successful](/blog_api/images/Kaustav_Set/5.List_All_Users_Successful.png)

**Read a User Data by ID:**

Here the details of the user with the specific id are returned, provided proper api-token is passed on.

![Retrieve_User_By_Id_Successful](/blog_api/images/Kaustav_Set/6.Retrieve_User_By_Id_Successful.png)

### UPDATE:

The objective of this section is to update the user data.
Here the user's name is changed, provided proper api-token is passed on, during the request. The updated user details are returned as follows:

![Name_Change_Successful](/blog_api/images/Kaustav_Set/4.Name_Change_Successful.png)

### DELETE:

The objective of this section is to delete the user.
Here the user is deleted, only if proper api-token is passed on, during the request. This activity is shown in this image:

![User_Delete_Successful1](/blog_api/images/Kaustav_Set/7.User_Delete_Successful1.png)

In order to check if the user is deleted or not, I tried to retrieve the details of the user with the same api-token. Received the error stating that "user does not exist, invalid token" , as expected. This is shown in the image below:

![User_Delete_Successful2](/blog_api/images/Kaustav_Set/8.User_Delete_Successful2.png)


Below is a screenshot of all the requests made to the app during the CRUD operations:


![All_Requests](/blog_api/images/Kaustav_Set/9.All_Requests.png)



