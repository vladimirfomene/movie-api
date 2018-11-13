# REST API with Spring WebFlux

## IDE and Tools

* I used Intellij IDE to develop this sample application.
* I created a skeleton of the project from [Spring Boot's bootstrap site](https://start.spring.io/)
* Specified Gradle as my build system and selected Security, Reactive Web, Reactive MongoDB and Embedded MongoDB for my dependencies.


## App Dependencies

* This app depends on Spring's Security, Reactive Web, Reactive MongoDB, Embedded MongoDB, `spring-security-oauth2-jose`
and `spring-security-oauth2-resource-server`.

## App Components

 * Created a representation of the API on Auth0 and secured it using Auth0's Authorization server.
 * REST API implemented using the Spring WebFlux API and Annotated Controllers.
 
 
 ## Running the App
 Run the app from a terminal by issuing the following command:
   
```bash
  ./gradlew bootRun
```


## Testing the application

Make sure you have `Curl` or `Postman` installed to test the endpoints of the API.

* To get all the movies from the API run the following command:

```bash
curl -v -X GET http://localhost:8080/movies
```

* To get a particular movie from the API.

```bash
curl -v -X GET http://localhost:8080/movies/{id}
```
where id corresponds to the `id` of anyone of the movie entries you got as result from the first request.

* To update a particular movie from the API.

```bash
curl -v -H "Authorization: Bearer <ACCESS-TOKEN>" -H "Content-Type: application/json" -X PUT -d
'{
         "id": "<Movie-ID-HERE>",
         "name": "<NEW-NAME",
         "genre": "<NEW-GENRE>",
         "releaseDate": "<NEW-DATE>"
     }' http://localhost:8080/movies/{id}

```
where id corresponds to the `id` of anyone of the movie entries you got as result from the first request.


* To delete a particular movie from the API.

```bash
curl -v -H "Authorization: Bearer <ACCESS-TOKEN>" -X DELETE http://localhost:8080/movies/{id}

```
where id corresponds to the `id` of anyone of the movie entries you got as result from the first request.

* Finally, to delete all the movies from the API.

```bash
curl -v -H "Authorization: Bearer <ACCESS-TOKEN>" -X DELETE http://localhost:8080/movies
```
where id corresponds to the `id` of anyone of the movie entries you got as result from the first request.