
# EXPERIMENT 1B

## AIM
File Sharing Within an Organization Using IP Address

## THEORY
In a local area network (LAN), computers communicate with one another using unique numeric identifiers called **IP (Internet Protocol) addresses**. File sharing within an organization relies on the **Server Message Block (SMB)** protocol over TCP/IP, which allows client applications to read and write to files on a host server.

## STEPS EXECUTED IN THEORY

1. **Host Network Identification:**  
   The host machine's IP address and network adapter details are retrieved using the network configuration command:
   ```cmd
   ipconfig
   ```

2. **Network Connectivity Verification:**
The connection stability and network latency between workstations are verified using the Internet Control Message Protocol (ICMP) echo request tool:
   ```cmd
    ping 10.17.60.44
    ```

3. **Directory Sharing Configuration:**
A target directory is configured on the host machine (`sit.lab2`) with active read/write permissions enabled under **Properties -> Sharing -> Advanced Sharing**.
4. **Remote Access via Universal Naming Convention (UNC):**
Client machines on the same subnet (`255.255.255.0`) connect directly to the shared resource over TCP/IP using the syntax:
    ```text
    \\10.17.60.44\Shared_Folder
    ```

## CONCLUSION
The network interface configurations were successfully retrieved using the ipconfig command, and IP connectivity was verified using the ping utility with a 0% packet loss rate. File sharing within the organization was established and executed using the host system's IP address (\\10.17.60.44).

The network interface configurations were successfully retrieved using the `ipconfig` command, and IP connectivity was verified using the `ping` utility with a 0% packet loss rate. File sharing within the organization was established and executed using the host system's IP address (`\\10.17.60.44`).
