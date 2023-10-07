## Project 0 Questions - Steven Choi

# Question 1 - ab requests in 10 seconds

Level 1: 26 requests
Level 2: 73 requests
Level 4: 159 requests
Level 8: 265 requests
Level 16: 385 requests
Level 32: 791 requests
Level 64: 730 requests
Level 128: 1145 requests
Level 256: 1275 requests

# Question 2

There are diminishing returns at higher concurrency levels because of factors such as overhead, context switching, and server resources. Generally in multi-threaded code, more threads may not always equal faster/more requests because context switching between threads take resources. And if the web server does not have the cores to support the number of concurrency levels, the time it takes to context switch may take longer than waiting for all the threads to finish the requests. As a result, the web server may not be able to allocate resources like CPU, memory, I/O efficiently. 

# Question 3

Level 1: 71 requests
Level 2: 178 requests
Level 4: 311 requests
Level 8: 620 requests

From the first few tests, we can see that http is already faster than https, and this makes sense because https must go through an SSL handshake, which can delay the loading speed.

# Question 4

Github can respond quickly likely because the static webpage site does not have a lot of traffic other than us and because Github has strong servers and infrastructure. 

# Question 5

My site's "Time to Interactive" is 0 ms.


