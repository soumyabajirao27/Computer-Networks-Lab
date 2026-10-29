# EXPERIMENT 9A

Implementation of Traffic Shaping Algorithm Using the Leaky Bucket Technique

## THEORY
The **Leaky Bucket algorithm** is used to control the rate at which traffic is injected into a network (traffic shaping). It handles bursty traffic by smoothing out traffic rates. Packets are stored in a bucket of a fixed capacity. If the bucket overflows, incoming packets are dropped (congestion control). Packets are leaked out from the bucket at a constant, fixed rate.

## TERMINAL SESSION
```
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ vim leaky_bucket_1290.c
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ gcc leaky_bucket_1290.c -o leaky_bucket
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ ./leaky_bucket
Enter bucket size: 10
Enter output rate (leak rate): 3
Enter number of packets to incoming queue: 4
Enter packet size for packet 1: 4
Enter packet size for packet 2: 5
Enter packet size for packet 3: 2
Enter packet size for packet 4: 3

--- Simulation ---
Incoming packet of size 4. Bucket status: 4/10
Incoming packet of size 5. Bucket status: 9/10
Incoming packet of size 2. Bucket overflow! Dropped packet of size 2.
Incoming packet of size 3. Bucket overflow! Dropped packet of size 3.

Leaking packets...
Leaked 3 packets. Remaining in bucket: 6
Leaked 3 packets. Remaining in bucket: 3
Leaked 3 packets. Remaining in bucket: 0
```

## CONCLUSION
The traffic shaping algorithm using the Leaky Bucket technique was successfully implemented in C. The algorithm effectively regulated bursty packet inputs, managed bucket capacity overflow, and leaked packets at a constant predefined rate.
