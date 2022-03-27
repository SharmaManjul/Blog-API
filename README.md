# Blog-API
REST API that allows you to access and edit blog posts and their authors using GET and POST commands. Blog-API 
is built using Spring and JPA written in Java.

###Endpoints
The endpoint of this API is: localhost/api/v1/posts . Navigate the posts using the post id appended after 
posts/

###Versioning
**API version**: The current version of this API is v1

**Entity version**: Ids of both posts and authors have etag versioning enabled which allows anyone to check if 
the post has been updated or is the first post. 

###Inner Workings
The project uses an interface for both the posts and authors which extends to the JPA repository. These 
interfaces allow us to work with the database loader which is used to add and save authors and posts. Both
the authors and posts are modeled individually as classes (entities) where we structure the attributes.
