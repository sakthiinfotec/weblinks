### Redis

[Top 5 use cases by Shan Lam](https://x.com/sahnlam/status/1713778548534845859)
    
  ![image](https://github.com/user-attachments/assets/455fe659-4f17-4672-8e39-61ffe6632195)
    
1. **Caching:** The most common use case is to utilize Redis for caching. This helps protect the database layer from overloading. Redis offers fast lookup times for cached data and can help improve application performance.

2. **Session Store:** We use Redis to share user session data among stateless servers. Redis provides a centralized place to store session data and makes it easy to scale out servers.

3. **Distributed lock:** We use Redis distributed locks to grant mutually exclusive access to shared resources. This prevents race conditions in distributed systems. Redis locks are easy to implement and automatically expire.

    Distributed Lock Implementations
    - **Redlock-py** (Python Implementation)
    - **Pottery** (Python Implementation)
    - **Aioredlock** (Asyncio Python Implementation)
    - **Redlock-php** (PHP Implementation)
    - **PHPReedisMutex** (further PHP Implementation)
    - **chepresov/php-redis-lock** [PHP library for locks)
    - **rtckit/react-redlock** (Async PHP Implementation)
    - **Redsync** (Go Implementation]
    - **Redisson** (Java Implementation)
    - **Redis::DistLock** [Perl Implementation)
    - **Redlock-cpp** [C++ Implementation)
    - **Redis-plus-plus** (C++ Implementation)

4. **Counter and Rate Limiter:** We use Redis to track like counts, view counts etc on social media apps. Redis counters provide atomic increments/decrements. We also use Redis to enforce rate limits on our API endpoints. This helps prevent abuse.

5. **Leaderboard:** Sorted sets make it easy to implement gaming leaderboards in Redis. We can add, update, or remove users from the leaderboard and query ranges efficiently.

[Top 5 Redis Use Cases by ByteByteGo](https://www.youtube.com/watch?v=a4yX7RUgTxI)
