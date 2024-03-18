## Active directory
```bash
  Active Directory (AD) is a Microsoft technology used in managing users, computers, and other devices on a network. It acts like a central hub, organizing and providing access to network resources like files, folders, printers, and more. Let's break down its components:
  
  ### Physical Components:
  
  1. **Data Store**: This is where all the information about users, computers, and network resources is stored. It's like a big database for your network.
  
  2. **Domain Controller**: Think of this as the boss of a specific area on the network, called a domain. It manages user logins, passwords, and access to resources within its domain.
  
  3. **Global Catalog Server**: This is like a special library that holds a summary of information about all the objects in the entire network. It helps in finding things quickly across different domains.
  
  4. **Read-only Domain Controller (RODC)**: This is a special type of domain controller that only stores read-only copies of the AD database. It's useful in remote locations with limited connectivity.
  
  ### Logical Components:
  
  1. **Partitions**: Imagine dividing your AD database into different sections, each containing specific types of information.
  
  2. **Schema**: Think of this as the blueprint or design of your AD database. It defines the types of objects (like users, computers) and the attributes (like name, email) they can have.
  
  3. **Domains**: Picture domains as separate neighborhoods in a city, each with its own rules and security settings. Users in one domain may not automatically have access to resources in another domain.
  
  4. **Domain Trees**: Imagine multiple neighborhoods (domains) connected together in a hierarchy, forming a tree-like structure. This allows for easier management and organization of resources.
  
  5. **Forests**: Think of forests as entire cities made up of multiple neighborhoods (domains) connected together. They share a common schema and global catalog.
  
  6. **Sites**: Picture different physical locations in your organization, like offices or branches. Sites help in organizing network traffic efficiently and applying specific settings based on location.
  
  7. **Organizational Units (OUs)**: These are like folders within domains where you can organize users, computers, and other objects based on departments, teams, or any other criteria you choose.
  
  **Example**:
  
  Let's say you work at a company called ABC Corp. In ABC Corp's Active Directory:
  
  - The data store is like the company's main filing cabinet where all employee information is kept.
  - Each office building has a domain controller managing access to resources within that building.
  - The global catalog server is like a library catalog that helps you find books (or network resources) quickly across different departments.
  - In the logical realm, imagine ABC Corp as a city. Each department (HR, IT, Sales) is like a neighborhood (domain) with its own rules and security.
  - These neighborhoods are organized into a tree structure (domain tree) with a common city plan (schema).
  - ABC Corp may have multiple cities (forests) if it has different branches or subsidiaries.
  - Sites help in managing network traffic efficiently between different office locations.
  - OUs are like filing cabinets within each department where you can organize employees based on teams or projects.
  
  Understanding these components helps in efficiently managing and organizing the network resources within an organization.
  
```
## LLMNR Poisoning 
```bash
    LLMNR stands for Link-Local Multicast Name Resolution. It's a protocol used in Windows networks when a device needs to find the IP address of another device on the same local network but doesn't know its IP address. For example, if you type a wrong network path in Windows Explorer, it may use LLMNR to try to find the correct device.

    LLMNR poisoning is when a malicious actor exploits LLMNR to redirect network traffic to their own device instead of the intended one. This can happen in an Active Directory environment, which is a type of network setup commonly used in businesses.

    Here's a simple example: Let's say you're in an office with multiple computers connected to the same network. You mistype a network address, and your computer sends out an LLMNR request asking, "Hey, does anyone know the IP address for this address?" Normally, the correct device would respond with its IP address. However, a hacker could intercept that request and respond with their own IP address, tricking your computer into sending its network traffic to the hacker's device instead of the intended one.

    This kind of attack can be used for various malicious purposes, such as stealing login credentials or redirecting users to fake websites. It's a threat to network security and can be used as a part of broader attacks on Active Directory networks.
```