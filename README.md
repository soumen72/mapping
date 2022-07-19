
# Mapping

One to Many,many to one Mapping Example with Spring Boot using a generic example


## Installation and run locally

Install mapping project with with the https pull

```bash
  
  Install jdk 17
  Install maven
  git clone {my project}
  cd mapping project //till the pom as root
  build the project
  mvn spring-boot:run


```
    
## API Reference

#### post a object (pass the parameter)

```http
  POST /posts
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `title,description,content` | `string` | **Required**. hit the endpoint to persist data |

#### Get item

```http
  GET /posts
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `None` | `string` | **Required**. get all posts, and all it's associted comment if any |

#### Get item


```http
  PUT /posts/{postId}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `postId`      | `string` | **Required**. Id of item to fetch and update , if exixt |

```http
  DELETE /posts/{postId}
```

| Parameter | Type     | Descriptiosn                       |
| :-------- | :------- | :-------------------------------- |
| `postId`      | `string` | **Required**. Id of item to fetch and detete |
#### Get item

```http
  GET /comments
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `None` | `string` | **Required**. get all comment and associated with which post |

```http
  POST /posts/{postId}/comments
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `postId` | `string` | **Required**. add a comment if the post exist |



```http
  GET /posts/{postId}/comments
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `postId` | `string` | **Required**. get all comment of a post |


#### add(num1, num2)

Takes two numbers and returns the sum.


## Screenshots
 Post add post

![App Screenshot](https://raw.githubusercontent.com/soumen72/mapping/master/images/Screenshot%202022-07-19%20at%202.16.56%20PM.png)

POST add comment for a post

![App Screenshot](https://raw.githubusercontent.com/soumen72/mapping/master/images/Screenshot%202022-07-19%20at%202.14.19%20PM.png)

GET all comment and their associated post

![App Screenshot](https://raw.githubusercontent.com/soumen72/mapping/master/images/Screenshot%202022-07-19%20at%202.14.30%20PM.png)


GET all posts

![App Screenshot](https://raw.githubusercontent.com/soumen72/mapping/master/images/Screenshot%202022-07-19%20at%202.13.46%20PM.png)


## Related

Here are some related projects, from where i got reference

[Source reference](https://www.callicoder.com/hibernate-spring-boot-jpa-one-to-many-mapping-example/)

