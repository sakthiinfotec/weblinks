### DNS
An A Record is a type of DNS record that maps a domain name to an IPv4 address. This makes it so that a difficult-to-remember IPv4 address (e.g. 203.0.113.1) translates to an easy-to-read, highly marketable domain name (e.g. example.com). You can point multiple A records to the same domain utilizing a different IPv4 address for redundancy or point multiple A records with different domain names to the same IPv4 address.

An A record consists of the following fields

- **Name:** Subdomain - usually appended with an @
- **TTL:** Time-to-live, the amount of time (in seconds) that the record is cached
- **Value/Address:** Target IPv4 address of the A record

- [Ref: How to Connect Your VPS to Your Domain Name](https://support.us.ovhcloud.com/hc/en-us/articles/360012042099-How-to-Connect-Your-VPS-to-Your-Domain-Name)  

### AWS Route 53

[Amazon Route 53](https://www.youtube.com/watch?v=RGWgfhZByAI) is a highly available and scalable cloud Domain Name System (DNS) web service or a DNS as a Service. It functions as the "phone book for the internet," translating human-readable domain names (like www.example.com) into numeric IP addresses that computers use to communicate.

Key features and benefits of Amazon Route 53 include:
- 100% availability ensuring consistent routing of end-users to applications.
- Seamless integration with other AWS services, allowing domain names to be mapped to resources like load balancers, EC2 instances, S3 buckets, and CloudFront distributions. It can also be used with non-AWS resources.
- Traffic Flow, which helps improve application performance and reliability by enabling easy setup of routing to send users to the best location and offering failover configurations to re-route users if a primary endpoint becomes unavailable.

### Relational Databases (SQL)
- **PostgreSQL**: Highlighted for its maturity, support for time series, and JSON/BSON (NoSQL) capabilities.
- **MySQL**: Mentioned for its ease of use.
- **SQLite**: Noted for being a flat file database, useful for local development without internet.

### NoSQL Databases
- **MongoDB**: Praised for its ease of use and lack of schema constraints.
- **DynamoDB**: Recognized for its scalability and cost-effectiveness, especially for high ingestion rates.

### Managed Database Hosting Providers
- **Supabase**: Offers a free PostgreSQL hosting solution, suitable for hobby or learner projects.
- **DigitalOcean Managed Databases**: Recommended for freelance projects due to its client management setup and developer experience.
- **Cloudflare D1**: A very cheap option for SQLite hosting.

These providers are noted for their low-cost and managed database hosting solutions.

### Infrastructure as a Code (IaaC)
- Infrastructure as a Code
- Network as a Code
- Policy as a Code
- Configuration as a Code
- Secutiry as as Code
