# EXPERIMENT 8

Implementation of Sliding Window Protocol Using Go-Back-N ARQ Technique

## THEORY
The **Go-Back-N ARQ (Automatic Repeat Request)** protocol is a sliding window protocol used at the Data Link or Transport layer for reliable data transfer. In this technique, the sender is allowed to transmit up to $N$ frames (where $N$ is the window size) without waiting for an acknowledgment. 

If an acknowledgment for a frame is not received or a frame is corrupted/lost, the sender retransmits that frame and **all subsequent frames** in the current window, ensuring ordered delivery.

## Terminal Session
```
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ vim sliding_window_1290.c
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ gcc sliding_window_1290.c -o sliding_window
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ ./sliding_window
Sliding Window Protocol Simulation (Go-Back-N)
Enter number of frames to send (max 50): 6
Enter window size: 3

Sender window: [0] [1] [2]
Sending frames...
Sent frame: 0
Sent frame: 1
Sent frame: 2

Simulating receiver...
Received frame: 0, sending ACK: 1
Received frame: 1, sending ACK: 2
Received frame: 2, sending ACK: 3

Did all frames receive correctly? (y/n): y

Sender window: [3] [4] [5]
Sending frames...
Sent frame: 3
Sent frame: 4
Sent frame: 5

Simulating receiver...
Received frame: 3, sending ACK: 4
Received frame: 4, sending ACK: 5
Received frame: 5, sending ACK: 6

Did all frames receive correctly? (y/n): y
All frames sent successfully!
```

## CONCLUSION
The sliding window protocol using the Go-Back-N ARQ technique was successfully implemented and simulated in C. The sender managed frame transmissions within the defined window size ($N=3$), tracked acknowledgments, and successfully completed transmission across sequential window batches.
