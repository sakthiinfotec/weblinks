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

### API gateways vs Load balancers

Load Balancers: Focus on distributing raw traffic to servers for balancing load.
API Gateways: Focus on application-level concerns such as request routing, authentication, and transformation.
API gateways handle the "what" (routing, security, transformation) of your API traffic, while load balancers handle the "how" (distribution, scalability, fault tolerance).

Load balancers can help you handle the influx of traffic by distributing requests to different servers to ensure a smooth user experience. In contrast, API gateways can handle tasks like authentication and authorization, helping you create a secure online shopping experience.

Load Balancer: Its main purpose is to distribute by load balancing traffic between multiple back end systems.
- We can configure different routes for different back end systems.
- We get a static ip address for the load balances end points (usually not available with API gateways)
- Can configure health checks (usually not available with API gateways)

API Gateways:
- Can implement rate limiting, bursting limits
- Can do request validation and request/response mapping
- Usually cloud API gateways allows to export/import cross API platform using swagger spec
- Allows caching responses

#### Static IP Address
A static IP address is needed when you require a consistent, unchanging internet address for a device or service, such as hosting a website, running a server, using a VPN, or accessing remote systems, as it allows other devices to reliably connect to your network without needing to constantly update their connection details due to a changing IP address; most regular internet users don't need a static IP as their basic browsing activities don't require a fixed address. 
Key reasons to use a static IP:
- **Server Hosting:** Websites and other servers need a stable IP address for users to consistently access them. 
- **Remote Access:** If you need to remotely access devices on your network, a static IP allows for easier configuration and access control. 
- **VPN Services:** Secure connections through a VPN often rely on whitelisting specific IP addresses, which is easier to manage with a static IP. 
- **VoIP (Voice over IP):** For reliable voice calls over the internet, a static IP is preferred to ensure consistent connection quality. 
- **Security Measures:** Some security systems utilize IP-based access controls that function better with a static IP. 
