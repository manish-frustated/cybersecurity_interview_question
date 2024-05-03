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

## OWASP Top 10 API Security Risks – 2023:
```bash
1. **Broken Object Level Authorization (API1:2023)**:
   - **Explanation**: This means that the API doesn't properly check if the user has permission to access certain data or objects.
   - **Example**: Imagine a banking API where users can view their account balance. If the API doesn't check if a user is authorized to view another user's balance, it's a broken object level authorization. So, User A could potentially see User B's balance.

2. **Broken Authentication (API2:2023)**:
   - **Explanation**: This is when the process that verifies a user's identity is flawed, allowing unauthorized users to access the system.
   - **Example**: If a shopping website's API doesn't properly verify user credentials during login, attackers might be able to access someone else's account just by guessing passwords or exploiting weaknesses in the authentication process.

3. **Broken Object Property Level Authorization (API3:2023)**:
   - **Explanation**: Similar to broken object level authorization, but focuses on specific properties or attributes of an object.
   - **Example**: In a social media API, if users can edit their own posts but the API doesn't check if they have permission to edit specific parts, like comments, it's a broken object property level authorization.

4. **Unrestricted Resource Consumption (API4:2023)**:
   - **Explanation**: This vulnerability allows attackers to use up all the resources available to an API, like memory or processing power, causing it to crash or become unavailable to legitimate users.
   - **Example**: A file-sharing API that doesn't limit the size or number of files a user can upload could be vulnerable to unrestricted resource consumption. An attacker could flood the API with large files, overwhelming its capacity.

5. **Broken Function Level Authorization (API5:2023)**:
   - **Explanation**: Similar to broken object level authorization, but focuses on specific functions or actions a user can perform.
   - **Example**: If a messaging app's API allows any authenticated user to delete messages, regardless of who sent them, it's a broken function level authorization.

6. **Unrestricted Access to Sensitive Business Flows (API6:2023)**:
   - **Explanation**: This vulnerability allows unauthorized users to access or manipulate critical processes or workflows within the system.
   - **Example**: An e-commerce API that lets anyone access the checkout process without proper authentication or authorization, potentially allowing them to manipulate orders or payments.

7. **Server Side Request Forgery (API7:2023)**:
   - **Explanation**: This is when an attacker can make the server perform actions on their behalf, often to access unauthorized resources or information.
   - **Example**: If an API allows users to input URLs for image processing, but doesn't properly validate those URLs, an attacker could input a URL that points to internal resources, like configuration files, leading to server-side request forgery.

8. **Security Misconfiguration (API8:2023)**:
   - **Explanation**: This occurs when security settings are not properly configured, leaving vulnerabilities open to exploitation.
   - **Example**: If an API's default passwords are not changed, or if unnecessary services are left running, it's a security misconfiguration.

9. **Improper Inventory Management (API9:2023)**:
   - **Explanation**: This vulnerability involves inadequate tracking or control of assets or resources within the system.
   - **Example**: A cloud storage API that doesn't properly track how much storage space each user is using could run out of space unexpectedly, affecting all users.

10. **Unsafe Consumption of APIs (API10:2023)**:
    - **Explanation**: This refers to using APIs in a way that exposes vulnerabilities or security risks.
    - **Example**: If an application uses a third-party API without verifying the data it receives, it could be vulnerable to injection attacks or other security exploits.
```