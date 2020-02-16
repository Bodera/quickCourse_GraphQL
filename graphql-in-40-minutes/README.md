## Learn GraphQL in 40 minutes

We will build a simple server-side API using GraphQL together with Node.js, the original tutorial was presented [here](https://youtu.be/ZQL7tL2S0oQ).

### A few words about what GraphQL is

If you are completely new to GraphQL you may be thinking that this is a brand new big complex thing, but in fact all GraphQL is a specific way of using tools that we already have. It is just a specification created around HTTP to obtain and receive resources from a server.

Usually you will work on something like REST when interacting with a server, and RESTful endpoints with the HTTP verbs (POST, GET, DELETE and UPDATE), all of these fun things to perform HTTP requests using REST. But GraphQL abstracts the whole idea of REST and all those different endpoints and provides a single endpoint and the way you determine what data you retrieve from that endpoint is based on the query that you send to that endpoint, rather thatoon which endpoint you send the data to. Now, let's look at an example of how a GraphQL query works compared to a REST query to get a better idea of the difference between the two.

### Spike user story

Imagine that you have an application that has books and authors as your two main resources, and each of these resources has maybe 13 fields in each, so let's assume the following you are creating a front-end application where you want to access only the author's name, all books and their names for that particular author and you want to display this in your application as soon as possible to your users.

- Book
  - id
  - Name
  - Genre
  - Page count
  - ISBN
  - authorId

- Author
  - id
  - Name

- - - -

Using a typical REST API endpoint as our first choice, we have two endpoints that we can use: the author's endpoint to get all the authors, and then a separate endpoint to get all the books from a particular author. Illustration provided below.

![Slide 01](WDS_Slides/sld-01.png)



