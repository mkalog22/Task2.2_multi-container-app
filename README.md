# multi-container app

Visit localhost:5000 in your browser to see the app in action. 

Refresh the page a few times—you’ll see the counter increase as each hit is recorded in Redis.


---


This multi-container application consists of an Express.js server and a Redis database, which run in separate containers. 

The Express.js server connects to the Redis database.

When the root URL ("/") is accessed, the server retrieves a counter value from Redis, increments it by one, stores the updated value back in Redis, and then responds with the updated counter value, displaying the number of page loads. This setup allows the application to keep track of the number of times the page has been loaded, storing the count persistently in Redis.
