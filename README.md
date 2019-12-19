# Web Application - Part 2

## Project Description

This project is all about creating an API for blogposts with methods to CREATE, GET_DETAILS, UPDATE_DETAILS, LIST_ALL_BLOGS, GET_A_BLOG_BY_ID and DELETE (CRUD methods). This homework is a part of the class IS 601 of Fall 2019.

## Problem Statement
For this assignment you need to follow this tutorial to create the application.

[https://www.codementor.io/olawalealadeusi896/building-a-restful-blog-apis-using-python-and-flask-part-2-l9y8awusp](https://www.codementor.io/olawalealadeusi896/building-a-restful-blog-apis-using-python-and-flask-part-2-l9y8awusp) 

Upload it to Github and submit a link to the repo branch called "part2"

## Output
I have created the API to supported the required CRUD operations and the images of the same are as follows:

### CREATE:

The objective of this section is to create a blogpost with title and contents. We can see in the image that the blog with the title "Welcome to Kaustav's blog" has been created the blog details are returned. But this will work only of the token of a logged in user is passed.

![Blogpost_Successful](/blog_api/images/part2/Kaustav_Set/1.Blogpost_Successful.png)

### READ:

The objective of this section is to read the blog details. This is achieved in the following ways:

**Read All Blog Details:**

Here the details of all the blogs are returned, provided proper api-token is passed on.

![Retrieve_All_Posts](/blog_api/images/part2/Kaustav_Set/2.Retrieve_All_Posts.png)

**Read a User Data by ID:**

Here the details of the blog with the specific id are returned, provided proper api-token is passed on.

![Retrieve_Post_By_Id](/blog_api/images/part2/Kaustav_Set/3.Retrieve_Post_By_Id.png)

### UPDATE:

The objective of this section is to update the blog data.
Here the blog's title and contents are appended with the term "Updated", provided proper api-token is passed on, during the request. An user can update only their blog. The updated blog details are returned as follows:

![Update_Post](/blog_api/images/part2/Kaustav_Set/4.Update_Post.png)

### DELETE:

The objective of this section is to delete ablog.
Here the blog is deleted, only if proper api-token is passed on, during the request.An user can delete only their blog. This activity is shown in this image:

![Post_Delete_Successful1](/blog_api/images/part2/Kaustav_Set/5.Post_Delete_Successful1.png)

In order to check if the blog is deleted or not, I tried to retrieve the details of that blog with the same api-token. Received the error stating that "post not found" , as expected. This is shown in the image below:

![Post_Delete_Successful2](/blog_api/images/part2/Kaustav_Set/6.Post_Delete_Successful2.png)


Below is a screenshot of some the requests made to the app during the CRUD operations:


![All_Requests](/blog_api/images/part2/Kaustav_Set/7.All_Requests.png)



