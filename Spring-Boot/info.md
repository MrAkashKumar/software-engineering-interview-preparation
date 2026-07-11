      Important Questions

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
      21) @Transactional present but rollback doesn't happen. Why?
      22) DB connection pool exhausts under load. Why?
      23) Scheduled jobs affect API latency. How to isolate?
      24) App behaves differently in Docker vs local. Why?
      25) New deployment but users see old behavior. What went wrong?
      26) Logs missing in production but present locally.
      Where to check?
      27) Async processing made performance worse. How?
      28) Circuit breaker stays open even when service is healthy. Why?
      29) Adding more resources didn't improve performance.
      Why?
      30) What Spring Boot decision you made could cause production issues?


      1. Why is String immutable in Java?
      2. What's the difference between HashMap and ConcurrentHashMap?
      3. How does HashMap handle collisions internally?
      4. When would you use volatile instead of synchronized?
      5. What causes a ConcurrentModificationException?
      6. How do you detect and resolve a deadlock?
      7. What's the difference between == and equals()?
      8. How does the JVM decide when to perform Garbage Collection?
      9. What causes an OutOfMemoryError, and how would you investigate it?
      10. What's the difference between ArrayList and LinkedList, and when would you choose each?
      11. How does the Executor Framework improve thread management?
      12. What happens internally when you call hashCode() and equals() in a HashMap?
      13. What's the difference between Callable and Runnable?
      14. How does CompletableFuture improve asynchronous programming?
      15. Why can a thread pool become exhausted even when CPU usage is low?
      16. What are the different types of JVM memory, and what is stored in each?
      17. What's the difference between fail-fast and fail-safe iterators?
      18. When would you use AtomicInteger instead of synchronized?
      19. How would you investigate a Java application that's becoming slower over time?
      20. If your Java application works perfectly in testing but randomly fails in production, what's your debugging approach?


      1. Why might @Transactional not roll back a transaction?
      2. How does Spring Boot auto-configuration work internally?
      3. What's the difference between @Component, @Service, and @Repository?
      4. How would you handle duplicate API requests in a payment service?
      5. What happens if two users update the same record simultaneously?
      6. How does Spring Boot manage database connections using HikariCP?
      7. What are the most common causes of connection pool exhaustion?
      8. How would you secure REST APIs using Spring Security and JWT?
      9. What's the difference between @PathVariable and @RequestParam?
      10. How would you improve a slow Spring Data JPA query?
      11. What is the N+1 query problem, and how do you fix it?
      12. How would you debug a Spring Boot application that's slow only in production?
      13. What's the difference between synchronous and asynchronous processing in Spring Boot?
      14. How would you prevent duplicate Kafka message processing?
      15. What's the purpose of Spring Boot Actuator, and which endpoints do you use most?
      16. How would you upload large files without causing memory issues?
      17. What's the difference between BeanFactory and ApplicationContext?
      18. How would you trace a request across multiple Spring Boot microservices?
      19. What steps would you take before scaling a Spring Boot application?
      20. If a production issue is reported but there are no exceptions in the logs, what's your debugging approach?

      A Senior Spring Boot interviewer asked only 3 questions.
      1. No coding.
      2. No theory.
      Just these:
      Scenario 1
            Your Spring Boot application works perfectly.
            After a deployment, only 5% of requests start failing randomly.
            Question: How would you identify the root cause without rolling back the deployment?
      --
      Scenario 2
            Customers report duplicate payments, but your logs show only one successful API request.
            Question: What could be happening behind the scenes?
      ---
      Scenario 3
            CPU is 18%, Memory is 45%, Database is healthy.
            Yet API latency suddenly jumps from 120ms to 9 seconds.
            Question: What's your debugging approach?


      -------------------------------------------
        Your API suddenly starts returning 503. What's your first check?
      • "@Transactional" isn't rolling back. Why?
      • HikariCP reports "Connection is not available." What's your debugging approach?
      • API latency jumps from 150ms to 5s after deployment. What could have changed?
      • Kafka consumer is alive, but lag keeps increasing. Why?
      • Duplicate orders are being created. How would you fix them?
      • Redis is serving stale data. What's your approach?
      • One microservice slows down the entire request chain. What would you investigate?
      • CPU is low, but response time is high. Why?
      • Your application works locally but fails only in production. Where do you start?
      • Memory usage keeps increasing every day. What's your first step?
      • Scheduled jobs start running twice after scaling. Why?
      • Health endpoint is UP, but users can't access the API. How is that possible?
      • Autoscaling creates more pods, but throughput doesn't improve. Why?
      • You have 20 minutes to identify the root cause of a production issue. What's your plan?


      1. Why can @Transactional fail even when no exception is thrown?
      2. Your Spring Boot API becomes slow only during peak hours. Where would you investigate first?
      3. How would you prevent duplicate order creation in a distributed system?
      4. Why can HikariCP run out of connections while the database is still healthy?
      5. A Kafka consumer is running, but lag keeps increasing. How would you debug it?
      6. Your application works locally but fails only in production. What's your first step?
      7. Why can a cache return stale data even after a successful database update?
      8. How would you investigate random 503 errors when all services appear healthy?
      9. Your scheduled job starts running twice after scaling. Why?
      10. How would you debug a memory leak in a Spring Boot application?
      11. One microservice is slowing down the entire system. How would you isolate it?
      12. Why does API latency increase while CPU and memory remain normal?
      13. What would you check before increasing the HikariCP pool size?
      14. How would you trace a request across multiple Spring Boot microservices?
      15. What's your first action when a production issue is reported but there are no exceptions in the logs?

      =========================================================================================================
      Your application is deployed on Kubernetes.
            Everything looks normal.
            - ✅ Pods are Running
            - ✅ Health checks are passing
            - ✅ Database is healthy
            - ✅ CPU usage is under 25%
            - ✅ Memory usage is normal
            
            But users suddenly start receiving 504 Gateway Timeout errors.
            
            The interviewer asked:
            1. What would you investigate first?
            2. Would you suspect Spring Boot or the infrastructure?
            3. Which logs would you check first?
            4. How would you determine whether the problem is in your application or a downstream service?
            5. What metrics would help you identify the root cause?
            6. Would you restart the pods immediately? Why or why not?
            7. How would you reproduce this issue without affecting production?
            8. Which Spring Boot Actuator endpoints would you use?
            9. If this happened every evening at 7 PM, what would you suspect?
            10. What's your step-by-step debugging approach?

      ==================================================================================
      21) @Transactional present but rollback doesn't happen.Why?
      22) DB connection pool exhausts under load. Why?
      23) Scheduled jobs affect API latency. How to isolate?
      24) App behaves differently in Docker vs local. Why?
      25) New deployment but users see old behavior. What went wrong?
      26) Logs missing in production but present locally.
      Where to check?
      27) Async processing made performance worse. How?
      28) Circuit breaker stays open even when service is healthy. Why?
      29) Adding more resources didn't improve performance. Why?
      30) What Spring Boot decision you made could cause production issues?

      ======================================================================================
      These are the most common reasons Spring Boot applications fail in production.

      1. High API latency
      → Check: Thread pool, HikariCP, slow SQL queries, external APIs.
      2. Database connection pool exhausted
      → Check: Connection leaks, long-running transactions, pool configuration.
      3. Memory keeps increasing
      → Check: Heap dump, unbounded cache, static collections, memory leaks.
      4. Random 503 errors
      → Check: Readiness probe, load balancer, downstream services.
      5. Duplicate records
      → Check: Retry logic, idempotency, race conditions.
      6. High CPU usage
      → Check: Infinite loops, excessive logging, expensive computations.
      7. High response time after deployment
      → Check: Cache warm-up, JVM JIT compilation, database execution plans.
      8. Scheduled job runs twice
      → Check: Multiple instances, distributed scheduler, locking mechanism.
      9. API works locally but fails in production
      → Check: Spring Profiles, environment variables, CORS, secrets.
      10. Everything looks healthy, but users still complain
      → Check: Business metrics, distributed tracing, logs, and external dependencies—not just Actuator health.

      If you see any of these, don't ignore them.
      1. CPU is low, but response time is high.
      → Think: Thread pool exhaustion, blocking I/O, downstream latency.
      2. Memory usage keeps growing every day.
      → Think: Memory leak, unbounded cache, object retention.
      3. Database is healthy, but HikariCP says "Connection is not available."
      → Think: Connection leaks, long-running transactions.
      4. 200 OK, but customers say the operation failed.
      → Think: Async processing, eventual consistency, external service failure.
      5. One pod is much slower than the others.
      → Think: JVM warm-up, uneven traffic, noisy neighbor.
      6. Kafka lag keeps increasing.
      → Think: Slow consumer, rebalance, downstream bottleneck.
      7. Autoscaling adds pods, but performance doesn't improve.
      → Think: Database bottleneck, locks, shared resources.
      8. GC pauses suddenly spike.
      → Think: Large object allocation, heap pressure, memory leak.
      9. API works locally but randomly fails in production.
      → Think: Environment differences, networking, secrets, configuration.
      10. Logs show everything is successful.
      Users still complain.


      21) @Transactional present but rollback doesn't happen. Why?
      22) DB connection pool exhausts under load. Why?
      23) Scheduled jobs affect API latency. How to isolate?
      24) App behaves differently in Docker vs local. Why?
      25) New deployment but users see old behavior. What went wrong?
      26) Logs missing in production but present locally.
      Where to check?
      27) Async processing made performance worse. How?
      28) Circuit breaker stays open even when service is healthy. Why?
      29) Adding more resources didn't improve performance.
      Why?
      30) What Spring Boot decision you made could cause production issues?

      
