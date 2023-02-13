# Exercise - Spring Boot - Interceptors-Middleware 1
* write a Spring Boot application with the necessary dependencies that:
  * has 2 controllers:
    * `BasicController` that:
      * is mapped on `time`
      * returns the current date/time
    * `LegacyController` that:
      * is mapped on `legacy`
      * returns `This is just old code`
  * has 2 interceptors/middleware:
    * `APILoggingInterceptor` that prints in the console the requests header `User-Agent`, before handling them
    * `LegacyIntercepotr` that:
      * blocks the API calls to the `legacy` endpoint
      * returns a response with the right HTTP code status for `Gone`
* test the 2 API endpoint calls using `Postman`
* **for reviewers**: `Postman`'s API calls collection is in `Interceptors-1.postman_collection.json` under the root
