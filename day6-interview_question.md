## Remote Procedure Call (RPC) protocol 135,593
```bash
   What is RPC?
   RPC stands for Remote Procedure Call. It's a protocol that allows one computer to execute code on another computer over a network.

   How does RPC work?
   RPC works like this:A program on one computer wants to execute code on another computer.
   It sends a request over the network to the remote computer.
   The remote computer receives the request, executes the code, and sends back the result.
   
   What are some examples of RPC on Windows systems?
   An example of RPC on Windows is when you share a printer over a network. When you print a document from your computer, it sends an RPC request to the computer where the printer is connected. That computer then processes the print job and sends back the result to your computer.
```
## NetBIOS Session Service 137,138,139
```bash
    Port 139 is typically associated with the NetBIOS Session Service (NetBIOS-SSN) on Microsoft Windows systems. NetBIOS (Network Basic Input/Output System) is an older networking protocol that allows applications on different computers to communicate within a local area network (LAN). NetBIOS-SSN is used for establishing sessions between computers for file and printer sharing, among other purposes. However, it's worth noting that NetBIOS is considered outdated and less secure compared to modern networking protocols.
```
## Microsoft-DS (Directory Services) 445
```bash
    Port 445 is commonly associated with the Microsoft-DS (Directory Services) service on Microsoft Windows systems. It's used for file and printer sharing, as well as other networking operations. The "microsoft-ds" service typically indicates a Windows operating system running in a workgroup environment with the name "WORKGROUP." This port is commonly open on Windows 7 through 10 systems for sharing files and resources across the network.
```
## Server Message Block (SMB) 139,445
```bash
    SMB is a network protocol used primarily for providing shared access to files, printers, and other resources on a network.
    It facilitates communication between client and server systems, allowing clients to access shared resources hosted on servers.
```

## note
```bash
    Sure, let's break it down in simple terms:

1. **NetBIOS-SSN**:
   - **What it does**: NetBIOS-SSN stands for NetBIOS Session Service. It's an older protocol used for communication between computers on a local network.
   - **Example**: Imagine two computers in the same office wanting to share files. NetBIOS-SSN helps them establish a connection to send and receive those files.

2. **Microsoft-DS (Directory Services)**:
   - **What it does**: Microsoft-DS is a specialized version of SMB developed by Microsoft. It's designed to work with Active Directory, a service used for managing users and resources in Windows networks.
   - **Example**: In a company network, Microsoft-DS helps computers communicate securely to access shared files, printers, and other resources managed by Active Directory.

3. **SMB (Server Message Block)**:
   - **What it does**: SMB is a networking protocol used for sharing files, printers, and other resources between computers on a network.
   - **Example**: When you share a folder on your computer with others in your home network, you're using SMB. It allows different devices to access and use the shared folder.

4. **msrpc**:
   - **What it does**: MSRPC (Microsoft Remote Procedure Call) is a protocol used by Windows for communication between processes on remote computers.
   - **Example**: Let's say you're using a program on your computer that needs to access data from another computer. MSRPC enables that program to request and receive the data over the network securely.

In summary, NetBIOS-SSN helps computers communicate locally, Microsoft-DS enhances SMB for Active Directory integration, SMB enables file and resource sharing on networks, and MSRPC facilitates communication between processes on remote computers in a Windows environment.
```