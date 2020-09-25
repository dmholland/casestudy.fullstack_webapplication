# My Blog

* **Description** - This is my blog that I got from https://nakov.com/blog/2016/08/05/creating-a-blog-system-with-spring-mvc-thymeleaf-jpa-and-mysql/ 
* **Features**- This is a skeleton/vanilla blog system and it allows freedom of speech.



### Project Configuration
* Ensure that you have mysql database installed on port 3306
  * Go inside of the resources/application.properties
  * Change the user to root
  * Put in your own password
  *Set server.ports to what you like

### Problems
* Project will not run on same database of two seperate deployments, will give errors: 'User name does not have a default' 
  * Passwords are not set to be very secure, so it is up to you to make strong passwords
  * Google will say 'Passwords for localhost:8080'
  * Put in your own password
  * Not set to delete users
  * Permissions are not set to anything but Admin, so anybody with access can delete other peoples posts
  * Need to set up permissions over posts. This is done through setting roles in spring security and changing permissions on edit, index, create pages.
  *Visitors can only see the last 5 posts. This can be enhanced.