# Computer Networks Laboratory (CN Lab)

Repository containing C programs, packet analysis documentation, and lab records for the Computer Networks Laboratory course.

---

## Laboratory Experiments Directory

| Exp No. | Experiment Name | Directory / Files |
| :---: | :--- | :--- |
| **1** | Study of Basic & Advanced Network Commands (`ping`, `ipconfig`, `tracert`, `netstat`, `nslookup`) | [`Exp 1/`](Exp%201/) <br>• `Exp 1A.md`<br>• `Exp 1B.md` |
| **2** | Count the number of comments, keywords, identifiers, words, lines and spaces from input file | [`Exp 2/`](Exp%202/) <br>• `Readme.md`<br>• `server_1290.c` |
| **3** | Socket Programming for Transport Layer Packets (TCP Server) | [`Exp 3/`](Exp%203/) <br>• `Readme.md`<br>• `client_1290.c` |
| **4** | Socket Programming for Transport Layer Packets (TCP Client) | [`Exp 4/`](Exp%204/) <br>• `Readme.md`<br>• `udp_server_1290.c` |
| **5** | Socket Programming for Transport Layer Protocol (UDP Client/Server) | [`Exp 5/`](Exp%205/) <br>• `Readme.md`<br>• `udp_client_1290.c` |
| **6** | Analysis of Application Layer Packets (DNS) Using Commands and Wireshark | [`Exp 6/`](Exp%206/) <br>• `Exp 6.md` |
| **7** | Analysis of Application Layer Packets (DNS & HTTP) Using Wireshark | [`Exp 7/`](Exp%207/) <br>• `Exp 7.md` |
| **8** | Implementation of Sliding Window Protocol Using Go-Back-N ARQ Technique | [`Exp 8/`](Exp%208/) <br>• `Readme.md`<br>• `sliding_window_1290.c` |
| **9A**| Implementation of Traffic Shaping Algorithm Using the Leaky Bucket Technique | [`Exp 9/Exp 9A/`](Exp%209/Exp%209A/) <br>• `Readme.md`<br>• `leaky_bucket_1290.c` |
| **9B**| Implementation of Traffic Shaping Algorithm Using the Token Bucket Technique | [`Exp 9/Exp 9B/`](Exp%209/Exp%209B/) <br>• `Readme.md`<br>• `token_bucket_1290.c` |
| **10**| Implementation of Distance Vector Routing Algorithm | [`Exp 10/`](Exp%2010/) <br>• `Readme.md`<br>• `distance_vector_1290.c` |

---

## Instructions for Execution

### 1. Compiling & Running C Programs
Navigate to any specific experiment folder containing a `.c` file and run:
```bash
gcc filename_1290.c -o program_output
./program_output
