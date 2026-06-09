      Questions

      1. How does Spring Boot auto-configuration work internally?

    2. What exactly happens when a Spring Boot application starts?
    
    3. Difference between @Component, @Service, @Repository, and @Controller?
    
    4. Why is constructor injection preferred over field injection?
    
    5. What is the bean lifecycle in Spring?
    
    6. Difference between BeanFactory and ApplicationContext?
    
    7. How does @Transactional work internally?
    
    8. What is propagation in transactions?
    
    9. Difference between Lazy Loading and Eager Loading?
    
    10. What is the N+1 problem in Hibernate? How did you solve it?
    
    11. Difference between CrudRepository and JpaRepository?
    
    12. How does Spring Data JPA create queries automatically?
    
    13. Difference between @RestController and @Controller?
    
    14. How does @RequestBody work internally?
    
    15. Difference between @PathVariable and @RequestParam?
    
    16. How do you handle global exception handling using @ControllerAdvice?
    
    17. Difference between Filters and Interceptors?
    
    18. How does Spring Security filter chain work?
    
    19. How JWT authentication works internally?
    
    20. Difference between authentication and authorization?
    
    21. How do microservices communicate with each other in your project?
    
    22. RestTemplate vs WebClient vs Feign Client?
    
    23. How did you implement Circuit Breaker in microservices?
    
    24. How do you handle distributed transactions in microservices?
    
    25. What problems did Kafka solve in your project?
    
    26. How do you avoid duplicate Kafka message processing?
    
    27. What happens if Kafka consumer crashes while processing data?
    
    28. How do you externalize configuration in Spring Boot?
    
    29. How do you troubleshoot slow APIs in production?
    
    30. What production issue did you face in Spring Boot and how did you fix it?

    
    1. Your Spring Boot application starts returning 500 errors after deployment. How will you debug it?
    2. You face BeanCreationException during application startup. What could be wrong?
    3. Your service throws NoSuchBeanDefinitionException in production but works locally. How will you fix it?
    4. You get CircularDependencyException between beans. How will you resolve it?
    5. Your API throws HttpMessageNotReadableException for valid requests. How will you debug it?
    6. You observe LazyInitializationException in production. How will you fix it?
    7. Your application fails due to incorrect configuration properties. How will you manage configs properly?
    8. You get DataIntegrityViolationException while saving data. What could be the issue?
    9. Your service throws TransactionRequiredException during updates. How will you handle transactions?
    10. Your API response time suddenly increases after enabling logging. How will you optimize it?
    11. You see memory leaks in your Spring Boot application. How will you detect and fix them?
    12. Your application fails to connect to the database intermittently. How will you debug it?
    13. You face timeout issues while calling another service. How will you handle it?
    14. Your application fails due to incorrect environment configuration. How will you manage profiles?
    15. You observe duplicate requests being processed. How will you ensure idempotency?
    16. Your service crashes due to unhandled exceptions. How will you implement global exception handling?
    17. You see high thread usage in your application. How will you optimize it?
    18. Your scheduled job runs multiple times unexpectedly. How will you fix it?
    19. Your application fails during deployment due to dependency conflicts. How will you resolve it?
    20. You observe inconsistent data due to concurrent transactions. How will you fix it?
    21. Your logs are insufficient to debug issues. How will you improve logging?
    22. Your API Gateway returns errors due to downstream failures. How will you handle it?
    23. Your application becomes unresponsive under load. How will you debug it?
    24. You need to deploy a new version without downtime. How will you achieve it?
    25. Your application behaves differently in production vs local. How will you approach debugging?

    1. Your Spring Boot application works fine locally but becomes slow in production with large database data. How will you identify and fix the issue?
    2. A database query suddenly starts taking 5x more time after deployment. How will you debug and optimize it?
    3. Your application runs out of database connections under high traffic. How will you resolve this?
    4. You notice duplicate entries in your database during concurrent requests. How will you prevent this?
    5. A transaction fails midway and leaves inconsistent data. How will you ensure proper rollback and consistency?
    6. Your service frequently faces deadlocks in the database. How will you detect and resolve them?
    7. After adding caching, users start seeing outdated data. How will you maintain cache consistency?
    8. Your database CPU usage is very high even with low API traffic. What could be the issue?
    9. A batch job processing large data fails in between. How will you make it fault-tolerant?
    10. Your API response time increases due to slow database calls. What optimizations will you apply?
    11. You need to handle millions of records efficiently. How will you design indexing and queries?
    12. A new schema change breaks existing queries in production. How will you handle backward compatibility?
    13. Your application shows random data inconsistencies across multiple tables. How will you debug this?
    14. Your database storage is growing rapidly and affecting performance. How will you manage it?
    15. A critical production issue occurs due to database failure. What is your recovery strategy?


      1. How does Spring Boot decide which **auto-configuration** to apply?
      2. What happens internally when you add 'spring-boot-starter-web'?
      3. Why does Spring Boot prefer **convention over configuration**?
      4. How does Spring Boot load 'application[dot]properties' internally?
      5. Exact **startup flow** of a Spring Boot application.
      6. Difference between '@ComponentScan' and @SpringBootApplication'
      7. How does Spring Boot detect **embedded Tomcat** and configure it?
      8. What happens if two beans of the same type exist without '@Qualifier'?
      9. How does Spring Boot handle **profile-specific configuration**?
      10. What is the role of 'SpringFactoriesLoader' under the hood?
      11. Difference between '@RestController' and '@Controller' internally.
      12. How does Spring Boot manage **dependency versions automatically**?
      13. Lifecycle of a Spring Bean in Spring Boot.
      14. How does Spring Boot handle **externalized configuration**?
      15. Fat jar vs normal jar — internal difference.
      16. How Spring Boot decides **server port priority**
      17. What happens internally when you hit a **REST endpoint**
      18. How Spring Boot integrates with **Actuator** internally.
      19. How exception translation works in Spring Boot.
      20. Common performance mistakes in Spring Boot applications.


    
