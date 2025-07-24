Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect to each other.

| **Routing Policy**    | **Use Case**                                                                                     |
| --------------------- | ------------------------------------------------------------------------------------------------ |
| **Simple**            | For a single resource (e.g., one web server). No special routing logic.                          |
| **Failover**          | For active-passive failover setups. Routes to a secondary resource if the primary is unhealthy.  |
| **Geolocation**       | Routes traffic based on the **user’s location** (e.g., country or continent).                    |
| **Geoproximity**      | Routes based on the **location of AWS resources**, with optional traffic shifting.               |
| **Latency**           | Routes to the region with the **lowest latency** for the user.                                   |
| **IP-based**          | Routes based on the **IP address** of the user, offering more granular control than geolocation. |
| **Multivalue Answer** | Returns up to **eight healthy records** randomly, useful for basic load balancing.               |
| **Weighted**          | Distributes traffic across multiple resources based on **custom weights** (percentages).         |
