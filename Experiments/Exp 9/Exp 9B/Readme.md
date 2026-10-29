# EXPERIMENT 9B

Implementation of Traffic Shaping Algorithm Using the Token Bucket Technique

## THEORY
The **Token Bucket algorithm** is another traffic shaping and congestion management technique. Unlike the leaky bucket (which forces a rigid output rate), the token bucket allows bursty traffic up to a certain maximum limit. Tokens are added to the bucket at a constant rate up to a maximum capacity. When a packet arrives, it must consume a designated number of tokens to be transmitted immediately. If insufficient tokens are available, the packet must wait or be discarded.

## TERMINAL SESSION
```
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ vim token_bucket_1290.c
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ gcc token_bucket_1290.c -o token_bucket
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ ./token_bucket
Enter maximum capacity of token bucket: 10
Enter initial tokens in bucket: 5
Enter token generation rate per interval: 2
Enter number of incoming packets: 3

Packet 1 requires 4 tokens.
Tokens available: 5. Packet transmitted successfully! Remaining tokens: 1

Packet 2 requires 6 tokens.
Not enough tokens! Adding generated tokens...
Current tokens: 3. Still insufficient tokens. Packet delayed or dropped.

Packet 3 requires 2 tokens.
Adding generated tokens...
Current tokens: 5. Tokens available: 5. Packet transmitted successfully! Remaining tokens: 3
```

## CONCLUSION
The traffic shaping algorithm using the Token Bucket technique was successfully implemented in C. The algorithm effectively managed token generation rates, supported burst capacity checks, and regulated packet transmissions based on available token credits.
