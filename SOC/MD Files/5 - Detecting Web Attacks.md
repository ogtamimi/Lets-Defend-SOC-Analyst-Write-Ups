# LECTURE5: Detecting Web Attacks

## 1) Introduction
Web applications are applications that provide services to users through a browser interface. 
Today, web applications make up a large part of internet usage. 
Sites such as Google, Facebook, and YouTube (excluding their 
mobile applications) are actually web applications.

## 2) Why Detecting Web Attacks Important

```
If we examine the anatomy of an attack, we can clearly see that 
the best scenario is to prevent the attack in its first phase. This is why there are various 
security measures aimed at preventing and detecting threats 
against web applications (WAF, IPS, SIEM rules...).
```

## 3) OWASP
The Open Worldwide Application Security Project (OWASP) is a 
non-profit foundation dedicated to improving software security.

### What is the name of the tool that OWASP has prepared to help scan web applications for vulnerabilities?
> **ANSWER: ZAP**
### Which area does OWASP focus on?
> **ANSWER: A**
### What is the name of the vulnerable web application project that OWASP wrote using Node.js for security researchers to improve themselves?
> **ANSWER: juice_shop**
### What does the OWASP Top 10 list, published every few years, reveal?
> **ANSWER: B**

## 4) How Web Applications Work
web applications communicate using the Hyper-Text Transfer Protocol (HTTP). 
Let's take a look at how the HTTP protocol works.

An HTTP request consists of a request line, request headers, and a request message body. 
The request line consists of the HTTP method and the resource requested from the web server. 
The request headers contain certain headers that the server will process. 
The request message body contains the data to be sent to the server.
```
--Status Line

The Status Line contains information about the HTTP version and the HTTP Response Status Code. 
The HTTP Response Status Code is used to describe the status of the request. 
There are many HTTP response status codes, but they can be summarized as follows:

● 100-199: Informational responses

● 200-299: Successful responses

● 300-399: Redirection messages

● 400-499: Client error responses

● 500-599: Server error responses
```

### What layer is HTTP on in the OSI model?
> **ANSWER: Application**
### Which HTTP Request header contains browser and operating system information?
> **ANSWER: User-Agent**
### What is the HTTP Response status code that indicates the request was successful?
> **ANSWER: 200**
### Which HTTP Request Method ensures that the submitted parameters do not appear in the Request URL?
> **ANSWER: POST**
### Which HTTP Request header contains session tokens?
> **ANSWER: Cookie**

## 5) Detecting SQL Injection Attacks
How to Prevent SQL Injections :

* Use a framework: Of course, just using a framework is not enough to prevent a SQL injection attack. However, 
it is still very important to use the framework according to the documentation.
* Keep your framework up to date: Keep your web application secure by following security updates according to the framework you use.
* Always sanitize data received from a user: Never trust data received from a user. In addition, sanitize all data (such as headers, URLs, etc.), not just form data.
* Avoid the use of raw SQL queries: You may be in the habit of writing raw SQL queries, but you should take advantage of the security provided by the framework.

### What date did the exploitation phase of SQL Injection Attack start?
> **ANSWER: 01/Mar/2022:08:35:14**
### What is the IP address of the attacker who performed the SQL Injection attack?
> **ANSWER: 192.168.31.167**
### Was the SQL Injection attack successful? (Answer Format: Y/N)
> **ANSWER: Y**
### What is the type of SQL Injection attack? (Classic, Blind, Out-of-band)
> **ANSWER: Classic**


## 6) Detecting Cross Site Scripting (XSS) Attacks 

Detecting XSS Attacks:

As we mentioned in the previous lesson, according to a study by 
Acunetix, 75% of cyber-attacks are conducted through web applications. As XSS is one of 
the most commonly tested vulnerabilities, you will 
encounter it throughout your career as a SOC analyst.

* Look for keywords: The easiest way to detect XSS attacks is to look for keywords such as "alert" 
and "script" that are commonly used in XSS payloads.
* Learn about commonly used XSS payloads: Attackers tend to use the same payloads to look for vulnerabilities before exploiting
an XSS vulnerability. Therefore, familiarizing yourself with commonly used XSS payloads would 
make it easier for you to detect XSS vulnerabilities. You can 
examine some commonly used payloads here.
* Check for the use of special characters: Check data coming 
from a user to see if any special
characters commonly used in XSS payloads, such as greater than 
(>) or less than (<), are present.

### What is the start date of the XSS attack?
> **ANSWER: 01/Mar/2022:08:53:20**
### What is the IP address of the attacker who performed the XSS attack?
> **ANSWER: 192.168.31.183**
### Was the XSS attack successful?
> **ANSWER: Y**
### What is the type of XSS attack? (Reflected, Stored, Dom based)
> **ANSWER: Reflected**


## 7) Detecting Command Injection Attacks 
How to Prevent Command Injection
--Always sanitize data you receive from a user: Never trust anything you receive from a user. Not even a file name!
--Limit user privileges: Whenever possible, set web application user rights at a lower level. 
Few web applications require users to have administrator rights. 
--Use virtualization technologies such as dockers.



### What is the date the command injection attack was initiated?
> **ANSWER: 01/Mar/2022:09:03:33**
### What is the IP address of the attacker who performed the Command Injection attack?
> **ANSWER: 192.168.31.156**
### Was the Command Injection attack successful?
> **ANSWER: N**


## 8) Detecting Insecure Direct Object Reference (IDOR) Attacks 

Insecure Direct Object Reference (IDOR) is a vulnerability caused 
by the absence or improper use of an authorization mechanism. It allows one person to access an object that belongs to another.

### What is the IP address of the attacker who carried out the IDOR attack?
> **ANSWER: 192.168.31.174**
### What is the date when the attack started?
> **ANSWER: 01/Mar/2022:11:42:32**
### Was the attack successful?
> **ANSWER: Y**
### Was the attack carried out by an automated tool?
> **ANSWER: N**

## 9) Detecting RFI & LFI Attacks 

--What is Local File Inclusion (LFI)?
Local File Inclusion (LFI), is the security vulnerability that 
occurs when a file is included without sanitizing the data obtained from a user. It differs 
from RFI because the file that is intended to be included is on the 
same web server that the web application is hosted on.

Attackers can read sensitive files on the web server, they can see the files containing 
passwords that would allow them to access the server remotely.


--What is Remote File Inclusion (RFI)?
Remote File Inclusion (RFI) is a vulnerability that occurs when a file is included without sanitizing 
the data received from a user. It differs from LFI because the included file is hosted on another server.

Attackers lure victims through websites on remote servers and trick them into
running malicious code on the servers they have prepared.

### What is the attacker's IP address?
> **ANSWER: 192.168.31.174**
### What is the start date of the attack?
> **ANSWER: 01/Mar/2022:11:58:35**
### Was the attack successful?
> **ANSWER: N**




## 10) Http Basic Auth Quix 

### How many HTTP GET requests are in pcap?
> **ANSWER: 5**
### What is the server operating system?
> **ANSWER: FreeBSD**
### What is the name and version of the web server software?
> **ANSWER: Apache/2.2.15**
### What is the version of OpenSSL running on the server?
> **ANSWER: OpenSSL/0.9.8n**
### What is the client's user-agent information?
> **ANSWER: Lynx/2.8.7rel.1 libwww-FM/2.14 SSL-MM/1.4.1 OpenSSL/0.9.8n**
### What is the username used for Basic Authentication?
> **ANSWER: webadmin**
### What is the user password used for Basic Authentication?
> **ANSWER: W3b4Dm1n**
# 100% CORRECT


## 11) Investigate Web Attack

### Which automated scan tool did attacker use for web reconnaissance?
> **ANSWER: Nikto**
### After web reconnaissance activity, which technique did attacker use for directory listing discovery?
> **ANSWER: Directory brute force**
### What is the third attack type after directory listing discovery?
> **ANSWER: Brute force**
### Is the third attack successful?
> **ANSWER: Yes**
### What is the name of fourth attack?
> **ANSWER: Code Injection**
### What is the first payload for 4th attack?
> **ANSWER: whoami**
### Is there any persistency clue for the victim machine in the log file ? If yes, what is the related payload?
> **ANSWER: %27net%20user%20hacker%20asd123!!%20/add%27**
# 100% CORRECT