      System Design => Important Design

    Step => 1
    https://github.com/ashishps1/awesome-system-design-resources

    Step => 2
    https://github.com/donnemartin/system-design-primer

    Step => 3
    https://github.com/ByteByteGoHq/system-design-101

    Step => 4
    https://github.com/karanpratapsingh/system-design

    Step => 5
    https://github.com/checkcheckzz/system-design-interview

    Step => 6
    Company - practical question
    https://github.com/systemdesign42/system-design-academy

    Step => 7
    https://github.com/InterviewReady/system-design-resources

    Step => 8
    https://github.com/chiphuyen/machine-learning-systems-design

    Step => 9
    https://github.com/sarwarbeing-ai/Agentic_Design_Patterns

    Step => 10
    https://github.com/binhnguyennus/awesome-scalability

    Step => 11
     => Company wise => 
    https://github.com/Jeevan-kumar-Raj/Grokking-System-Design

    Step => 12
    => Impro
    https://github.com/karanpratapsingh/system-design

    Step => 13
    => Company wise => 
    https://github.com/javabuddy/best-system-design-resources

    Step => 14
    https://github.com/yangshun/tech-interview-handbook


    https://medium.com/javarevisited/10-best-github-repositories-to-prepare-for-system-design-interviews-6cc9d37d50f6

    Thank You


    
      System Design Key Concepts: 
      
      1. Scalability: https://lnkd.in/gpge_z76
      2. Latency vs Throughput: https://lnkd.in/g_amhAtN
      3. CAP: https://lnkd.in/g3hmVamx
      4. ACID Transactions: https://lnkd.in/gMe2JqaF
      5. Rate Limiting: https://lnkd.in/gWsTDR3m
      6. API Design: https://lnkd.in/ghYzrr8q
      7. Strong vs Eventual Consistency: https://lnkd.in/gJ-uXQXZ
      8. Distributed Tracing: https://lnkd.in/d6r5RdXG
      9. Synchronous vs. asynchronous communications: https://lnkd.in/gC3F2nvr
      10. Batch Processing vs Stream Processing: https://lnkd.in/g4_MzM4s
      11. Fault Tolerance: https://lnkd.in/dVJ6n3wA
      
      ➤ System Design Building Blocks:
      
      1. Database: https://lnkd.in/gti8gjpz
      2. Horizontal vs Vertical Scaling: https://lnkd.in/gAH2e9du
      3. Caching: https://lnkd.in/gC9piQbJ
      4. Distributed Caching: https://lnkd.in/g7WKydNg
      5. Load Balancing: https://lnkd.in/gQaa8sXK
      6. SQL vs NoSQL: https://lnkd.in/g3WC_yxn
      7. Database Scaling: https://lnkd.in/gAXpSyWQ
      8. Data Replication: https://lnkd.in/gVAJxTpS
      9. Data Redundancy: https://lnkd.in/gNN7TF7n
      10. Database Sharding: https://lnkd.in/gMqqc6x9
      11. Database Index's: https://lnkd.in/gCeshYVt
      12. Proxy Server: https://lnkd.in/gi8KnKS6
      13. WebSocket: https://lnkd.in/g76Gv2KQ
      14. API Gateway: https://lnkd.in/gnsJGJaM
      15. Message Queues: https://lnkd.in/gTzY6uk8
      
      ➤ System Design Architectural Patterns:
      
      1. Event-Driven Architecture: https://lnkd.in/dp8CPvey 
      2. Client-Server Architecture: https://lnkd.in/dAARQYzq
      3. Serverless Architecture: https://lnkd.in/gQNAXKkb
      4. Microservices Architecture: https://lnkd.in/gFXUrz_T
      
      ➤ Low-Level Design Problems:
      
      1. Design Parking Lot: https://lnkd.in/dQaAuFd2
      2. Design Splitwise: https://lnkd.in/dF5fBnex
      3. Design Chess Validator: https://lnkd.in/dfAQHvN4
      4. Design Distributed Queue | Kafka: https://lnkd.in/dQ6_B4_M
      
      ➤ System Design and Architecture (HLD):
      
      1. Design Unique ID Generator Service
      2. Design bitly
      3. Design Whatsapp
      4. Design Insta/Twitter News Feed
      5. Design Search Autocomplete

      Question- 1 -> How can we create 100% unhackable application where must configured mechanishm - RASP -> Runtime Application Self-Protection 
      Question - 2 -> Design a RAG Pipeline for 10 million docs with zero hallucination.
      Question - 3 -> Ralph Wiggum loop pattern 
      Question - 4 -> Design an AI agent where answer user queries, Decide when to use external tools and remember past conversations
      Question - 5 -> Suppose you have to train a tiny language model with a mixture of K datasets but you do not know the optimal weight each 
                        dataset. your goal is to find these optimal weights to minimize the cross entropy on a validation set. how do you do this?
      Question - 6 -> 



🚦 Design a Distributed Rate Limiter | Senior+ System Design Walkthrough

One of the most common Senior Software Engineer (L5/L6) system design questions is:
"Design a Distributed Rate Limiter."
It sounds simple, but interviewers are actually evaluating your understanding of:

✅ Distributed Systems
✅ Scalability
✅ Atomic Operations
✅ Distributed Coordination
✅ Consistency vs Availability
✅ Performance Trade-offs

📝 Step 1: Clarify Requirements
Before designing, ask:
• Are we limiting per IP, User, API Key, or Endpoint?
• Is the limit per second, minute, or hour?
• Should it be a Hard Limit or Soft Limit (bursts allowed)?
• Does it run inside every service or as a central API Gateway/Middleware? (Preferred)
• Target latency? Ideally <1 ms p99, since it's in the hot path.

📊 Step 2: Capacity Planning
Imagine:
• 50,000 API servers
• 10K requests/sec each
➡️ 500 Million Requests/sec
A single Redis instance cannot handle this. The solution is to shard counters by API Key across a Redis cluster.

⚙️ Core Algorithms
1️⃣ Fixed Window Counter
✔ O(1) memory & computation
❌ Suffers from the boundary burst problem (users can exceed limits around window resets).

2️⃣ Sliding Window Log
✔ Perfect accuracy
❌ Stores every request timestamp, making memory usage expensive at scale.

3️⃣ Sliding Window Counter ⭐ (Recommended)
Maintains only:
• Current Window Counter
• Previous Window Counter
Estimated Count = Previous × Remaining Weight + Current
✅ O(1) memory
✅ Near-perfect accuracy
✅ Eliminates boundary burst
✅ Excellent for strict API rate limiting
This approach is widely associated with Cloudflare's production discussions.

4️⃣ Token Bucket
Each client owns a bucket of tokens.
• Every request consumes one token.
• Tokens refill continuously.
✅ Supports controlled bursts
✅ Great user experience
Ideal when short bursts are allowed while maintaining a long-term average.

5)🏗️ Distributed Challenges
The real challenge isn't counting requests—it's maintaining a global limit across thousands of servers.
Key considerations:
• Atomic Redis operations (INCR/Lua Scripts)
• Consistent Hashing
• Redis Sharding
• Replication & High Availability
• Multi-region synchronization
• Avoiding Single Points of Failure
