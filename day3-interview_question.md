## xss

```bash
  XSS stands for Cross-Site Scripting. It's a type of cyber attack where malicious scripts are injected into web pages viewed by other users. Imagine you have a comment section on a website. If a hacker manages to input a script into their comment, anyone else who views that comment might unknowingly execute the script, allowing the attacker to steal cookies or session tokens, redirect users to malicious websites, or deface the website. 
```

## Absolute and Relative Paths in Linux File System:

```bash
  Absolute Path: Specifies the exact location of a file or directory from the root directory. For example, /home/user/documents/file.txt.
  
  Relative Path: Specifies the location of a file or directory relative to the current working directory. For example, if your current directory is /home/user, then documents/file.txt is a relative path to access the same file.
```

## Directory Traversal Attack 

```bash
   This is a type of attack where an attacker tries to access files and directories that are outside of the web server's root directory. For example, if a website allows users to input a file name for download without proper validation, an attacker might input ../../etc/passwd which could lead to the server disclosing sensitive system files. 
``` 

## SSH: 

```bash
   SSH stands for Secure Shell. It's a cryptographic network protocol used for secure communication over an unsecured network. It's commonly used for remote access to computer systems, allowing users to log into and execute commands on a remote machine securely.
```

## Local File Inclusion:

```bash
   Local File Inclusion (LFI) is a type of vulnerability that allows an attacker to include files on a server through the web browser. For example, if a website includes files based on user input without proper validation, an attacker might manipulate the input to include sensitive files, leading to data exposure or remote code execution.
```
## Local File Inclusion v/s Directory Traversal :

```bash
   The main difference between LFI and Directory Traversal is the way in which files are accessed. In LFI, the attacker includes files directly through the web application, exploiting improper input validation. In Directory Traversal, the attacker traverses the directory structure to access files outside of the web server's root directory.
```

## Shells:

```bash
   Shells are command-line interfaces that allow users to interact with the operating system. Here's a brief overview of some common shells:

   Bash (Bourne Again Shell): This is the default shell for most Linux distributions. It's a powerful and versatile shell with many features for scripting and interactive use.
   
   Sh (Bourne Shell): One of the earliest Unix shells, it's a simple shell with basic functionality. It's lightweight and suitable for scripting.
   
   Zsh (Z Shell): An extended version of the Bourne shell with additional features like advanced tab completion and improved scripting capabilities.
   
   Fish (Friendly Interactive Shell): A user-friendly shell with features like syntax highlighting, autosuggestions, and a powerful scripting language.
   
   Csh (C Shell): Another early Unix shell, known for its C-like syntax and interactive features.
   
   Tcsh (TENEX C Shell): A variant of the C shell with additional features like command-line editing and job control.
```

## PHP wrappers

```bash
   PHP wrappers can be a valuable tool when assessing web applications for security vulnerabilities, including Local File Inclusion (LFI)
   PHP wrappers are special protocols that allow PHP functions to access various resources, including local files.
   By leveraging PHP wrappers, a penetration tester can exploit LFI vulnerabilities to read sensitive files on the server.

   Example scenario :
   Suppose a web application has an LFI vulnerability that allows an attacker to include arbitrary files.
   The attacker can craft a request using a PHP wrapper, such as php://filter/convert.base64-encode/resource=/etc/passwd.
   The server will interpret this as a request to read the /etc/passwd file, encode it in base64, and return the result.
   The attacker can then decode the base64 output to obtain information about system users.
```

## Remote File Inclusion (RFI) Attack:

```bash
   This attack is about making a website load a file from somewhere else, usually a bad place controlled by the hacker.
   Think of it like this: You're inviting someone over for dinner, but instead of bringing food, they bring a virus. That's what happens in an RFI attack.
   For example, if a website loads a file like this: http://example.com/loadfile.php?file=badstuff.php, the hacker can make it load their malicious file instead of the real one.

   Difference Between RFI and Local File Inclusion (LFI) Attack:

   RFI is when the hacker tricks the website into loading a file from somewhere else, usually controlled by the hacker. It's like inviting a virus into your system.
   LFI is a bit different. It's when the hacker tricks the website into showing a file that's already on the server, usually by manipulating the URL. So, instead of bringing in a virus from outside, they're just showing something nasty that's already there.
   Imagine you're reading a book, and the hacker swaps out a page in the book with something inappropriate. That's LFI.
```
