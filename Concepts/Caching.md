 #concepts #caching #strategies #terminology 

What is caching?
?
Caching is a technique used in computing to store and retrieve frequently accessed or computed data in a way that allows faster access when the same data is needed again. The primary goal of caching is to improve system performance by reducing the time and resources required to fetch or compute data.
Imagine you have a bookshelf, and every time you want to read a specific book, you go to the library to get it. Caching is like having a small shelf next to your favorite reading spot where you keep the books you read most often. This way, you don't need to go all the way to the library every time you want to read one of those books because they are already nearby.
In summary, caching is a strategy to make data access faster by keeping a copy of frequently used data in a faster storage location, reducing the need to fetch it from slower storage every time it's needed.

We can store data in cache, RAM and on disk. What are the differences?
?
- **Cache:** It's a small, high-speed storage area that stores a copy of data that is frequently accessed or computed.
- **Main Memory (RAM):** This is like the larger library where all the books (data) are stored. Accessing data from main memory is faster than fetching it from slower storage like a hard drive.
- **Storage (Hard Drive, Database):** This is like the library where all the books (data) are kept. Accessing data from storage is slower compared to accessing it from the cache or main memory.

How does caching work?
?
1. **First Access:**
   - When you first access data, it's fetched from the slower storage (library) and placed in the cache.
2. **Subsequent Access:**
   - If you need the same data again, instead of going back to the slower storage, the system checks the cache first.
   - If the data is in the cache (on your small shelf), it's retrieved quickly.

What are the benefits of caching?
?
1. **Faster Access:** Caching reduces the time it takes to access frequently used data since it's stored in a faster, closer location.
2. **Improved Performance:** Systems can respond more quickly to user requests, leading to better overall performance.
3. **Reduced Load on Resources:** Caching helps reduce the load on slower storage systems, like databases or hard drives, by serving frequently requested data from a faster cache.

What are examples of caching?
?
1. **Web Browsers:** Cached images, scripts, and stylesheets from websites are stored locally to speed up page loading on subsequent visits.
2. **Databases:** Frequently accessed database query results can be cached to avoid repeating the same expensive queries.
3. **Content Delivery Networks (CDNs):** CDNs cache static content (like images and videos) closer to users, reducing the load time for websites.