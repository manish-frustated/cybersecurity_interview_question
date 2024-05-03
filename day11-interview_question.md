## What is an API?

```bash
An API, or Application Programming Interface, is like a waiter in a restaurant. It helps two different software systems communicate and exchange information. Just like how you order food from a menu, software systems use APIs to request and send data between each other.
```

## Types of APIs:
```bash
RESTful APIs: These are the most common type of APIs. They use standard HTTP methods like GET, POST, PUT, PATCH, and DELETE to perform actions on resources. They are easy to understand and widely used on the web.
SOAP APIs: SOAP stands for Simple Object Access Protocol. These APIs use XML for message formatting and are often used in enterprise systems.
GraphQL APIs: GraphQL is a query language for APIs. It allows clients to request exactly the data they need and nothing more, which can be more efficient than RESTful APIs in certain situations.
```

## API Methods:

```bash
GET: This method is used to retrieve data from the server. It's like asking for the menu in a       restaurant. For example, when you visit a website, your browser sends a GET request to the server to get the web page.

POST: This method is used to send data to the server to create a new resource. It's like placing an order in a restaurant. For example, when you fill out a form on a website and submit it, your browser sends a POST request to the server with the form data.

PUT: This method is used to update an existing resource on the server. It's like asking the waiter to replace your order with something else. For example, when you edit your profile information on a website and save it, your browser sends a PUT request to update your profile on the server.

PATCH: This method is used to partially update an existing resource on the server. It's like asking the waiter to add some extra toppings to your order. For example, when you edit just your email address on a website and save it, your browser sends a PATCH request to update only the email address in your profile on the server.

DELETE: This method is used to delete a resource from the server. It's like asking the waiter to take your order off the table. For example, when you delete a post on a social media website, your browser sends a DELETE request to remove the post from the server.
```

## OWASP Top 10 API Security Risks – 2019:
```bash
1. **API1 Broken Object Level Authorization**: This means that the API doesn't properly check if you're allowed to access certain data. For example, let's say there's an API for a bank and you're only supposed to see your own account details. But if the API doesn't check properly, you might be able to see someone else's account details.

2. **API2 Broken User Authentication**: This happens when the API doesn't properly check if you're really the person you say you are. For instance, imagine a social media API that lets you post updates. If it doesn't check your login properly, someone else might be able to post as you.

3. **API3 Excessive Data Exposure**: This means the API gives out more information than it should. For example, a shopping website's API might reveal customer addresses when it's only supposed to show their names.

4. **API4 Lack of Resource and Rate Limiting**: If an API doesn't have limits on how much data you can access or how often you can access it, it could be overwhelmed with requests. Imagine a ticket booking API that doesn't limit how many tickets you can check at once. Someone could flood the system with requests, causing it to crash.

5. **API5 Broken Function Level Authorization**: Similar to Broken Object Level Authorization, but here it's about specific functions within the API. For example, an API might have a function to delete posts, but if it doesn't check properly, anyone could delete any post, not just their own.

6. **API6 Mass Assignment**: This occurs when an API allows too much data to be modified at once. Imagine an API for updating user profiles where you can change your email, password, and username. If it's not properly secured, someone might be able to change other users' information as well.

7. **API7 Security Misconfiguration**: This happens when the settings of the API are not set up securely. For example, if the API is supposed to be accessed over HTTPS for encryption but is mistakenly set to HTTP, it could expose sensitive data.

8. **API8 Injection**: Injection vulnerabilities occur when untrusted data is sent to an interpreter as part of a command or query. An example is SQL injection, where attackers can manipulate a database query to gain unauthorized access to data or even delete data.

9. **API9 Improper Asset Management**: This is about not properly managing the resources and assets used by the API. For example, leaving old or unused code or files accessible could provide avenues for attackers to exploit vulnerabilities.

10. **API10 Insufficient Logging & Monitoring**: If an API doesn't keep track of what's happening (logging) or doesn't actively watch for suspicious activity (monitoring), it might not notice if someone is trying to attack it. This could lead to security breaches going unnoticed for a long time.
```
## OWASP Top 10 API Security Risks – 2023:
```bash
1. **Broken Object Level Authorization**: This means that the API doesn't properly check if a user has the right to access certain objects or data. For example, let's say a banking API doesn't check if a user has permission to access another user's account information. So, anyone could access sensitive data without proper authorization.

2. **Broken Authentication**: This happens when the authentication process is flawed, allowing unauthorized users to gain access. An example would be an API that doesn't properly verify user credentials, allowing anyone to log in without a valid username and password.

3. **Broken Object Property Level Authorization**: Similar to Broken Object Level Authorization, but this specifically refers to the access control on individual properties or attributes of an object. For instance, if a healthcare API doesn't properly restrict access to a patient's medical history, allowing unauthorized users to view sensitive information like diagnoses or treatments.

4. **Unrestricted Resource Consumption**: This means that an API doesn't limit the resources (like CPU, memory, or bandwidth) that a single user can consume, making it vulnerable to denial-of-service attacks. For example, if an image processing API doesn't have limits on the size or number of images a user can upload, it could be overwhelmed by a flood of large files, causing it to crash or become unresponsive.

5. **Broken Function Level Authorization**: This occurs when certain functions within the API are accessible to users who shouldn't have permission to use them. For instance, if a file storage API allows any user to delete files, regardless of their permissions or role.

6. **Unrestricted Access to Sensitive Business Flows**: This means that the API allows users to access critical business processes or workflows without proper authentication or authorization. For example, if an e-commerce API allows users to bypass payment authentication and place orders without paying.

7. **Server Side Request Forgery**: This vulnerability allows an attacker to manipulate the server into making unintended requests to other servers. For example, an API that allows users to input URLs for fetching data, without proper validation, could be exploited to access internal systems or sensitive information on other servers.

8. **Security Misconfiguration**: This refers to insecure configurations in the API server or infrastructure, making it easier for attackers to exploit vulnerabilities. For example, leaving default passwords or unnecessary ports open on the server.

9. **Improper Inventory Management**: This means that the API doesn't properly track or manage its assets or resources, leading to vulnerabilities like outdated software versions or unpatched security flaws. For instance, if a software update API doesn't keep track of which clients have installed the latest patches, leaving some systems vulnerable to known exploits.

10. **Unsafe Consumption of APIs**: This refers to vulnerabilities caused by how the API consumes or interacts with other APIs or external resources. For example, if a weather API doesn't properly validate data received from another weather service before using it, allowing malicious data to cause unexpected behavior or security breaches.
```