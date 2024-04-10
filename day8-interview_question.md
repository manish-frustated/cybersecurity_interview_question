## Android system architecture layers

```bash
  Layer 1: Linux Kernel: This is the core of the Android operating system, providing low-level system functionalities such as process management, memory management, and hardware drivers. In terms of penetration testing, vulnerabilities at this layer could include privilege escalation exploits or vulnerabilities in device drivers. For example, an attacker might exploit a vulnerability in the Linux kernel to gain root access to the device.

    Layer 2: Libraries (and Libraries Runtime): This layer includes various libraries required for running applications, such as the C standard library (libc), SQLite library for database operations, and SSL libraries for secure communication. Penetration testing at this layer involves identifying vulnerabilities in these libraries that could be exploited by malicious apps. For instance, a vulnerability in the SSL library could lead to sensitive data being intercepted by an attacker during secure communication.

    Layer 3: Application Framework: This layer provides high-level building blocks for developing Android applications, including components like activities, services, and content providers. Penetration testing here involves assessing the security of these components for potential vulnerabilities such as insecure data storage or improper input validation. For example, an attacker might exploit a vulnerability in an Android activity to perform unauthorized actions or access sensitive data.

    Layer 4: Applications: These are the actual user-facing applications installed on the Android device. Penetration testing at this layer involves assessing the security of individual apps for vulnerabilities such as insecure data transmission, weak authentication mechanisms, or improper session management. For instance, a banking app might have a vulnerability that allows an attacker to steal login credentials or perform unauthorized transactions.
```
## Android terminologies

```bash
  Activity:
    Explanation: An Activity is like a window in your Android app. It represents a single screen with a user interface where users can interact.
    Example: Think of an Activity as a page in a book. Each page represents a different Activity, and you can flip between them to access different parts of the book (your app).
    
    Content Provider:
    Explanation: A Content Provider manages access to a structured set of data. It acts as a bridge between your app and a central data store.
    Example: Suppose you have an app that stores contacts. The Content Provider allows other apps to read and write to your contact list securely.

    Content Resolver:
    Explanation: A Content Resolver helps you query and manipulate data managed by a Content Provider. It acts as a middleman between your app and the Content Provider.
    Example: If your app wants to retrieve a list of contacts stored by another app, it uses a Content Resolver to communicate with the respective Content Provider.
    
    Broadcast Receiver:
    Explanation: A Broadcast Receiver is like an ear for your app. It listens for broadcast messages sent by the system or other apps.
    Example: Imagine your app needs to respond when the battery is low. You can create a Broadcast Receiver that listens for the "battery low" message and triggers an action, like showing a notification to the user.
    
    Intent:
    a. Explicit Intent: Specifies a particular component (like Activity or Service) that should be started.
    b. Implicit Intent: Requests an action to be performed by another component, without specifying the exact component.
    Explanation: Intents are messages that allow components to request functionality from other components within the same app or different apps.
    Example:
    Explicit: Opening a specific Activity when a button is clicked.
    Implicit: Asking the system to open a web page, letting the system choose which browser to use.
    
    Intent Filter:
    Explanation: An Intent Filter specifies the types of intents a component can respond to. It describes the capabilities of the component.
    Example: If your app has an Activity that can share images, you can define an Intent Filter to specify that your Activity can handle "image/*" MIME types.

    Intent Resolution:
    Explanation: Intent Resolution is the process by which the system decides which component should handle an incoming intent, especially implicit intents.
    Example: When you request to share an image, the system checks all apps that can handle image sharing and presents you with a list of options.

    Services:
    Explanation: Services are components that run in the background to perform long-running operations or to perform work for remote processes.
    Example: Playing music in the background while you use other apps is typically done by a Service. It runs independently of the user interface, ensuring music continues even if you switch to another app.
```
