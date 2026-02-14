# LECTURE4: Phishing Email Analysis


## 1) Introduction to Phishing

> **ANSWER: CHECK**
## 2) Information Gathering

```
Spoofing
Because emails do not necessarily have an authentication mechanism, 
attackers can send emails in the name of someone else. 
Attackers can do this by using a technique called spoofing to make 
the user believe that the incoming email is reliable. Several protocols have been created to prevent the email spoofing technique. 
The SPF, DKIM, and DMARC protocols can be used to determine whether 
the sender's address is fake or real. Some email programs check emails automatically. 
However, the use of these protocols is not mandatory and can cause 
problems in some cases.

--Sender Policy Framework (SPF)
--DomainKeys Identified Mail (DKIM)

To manually determine if a mail is spoofed or not, 
the SMTP address of the mail should first be identified. 
The domain's SPF, DKIM, DMARC, and MX records can be obtained using 
tools such as Mxtoolbox. 
Comparing this information will tell you if the email is spoofed or not.
```
> **ANSWER: CHECK**


## 3) What is an Email Header and How to Read Them?

```
What is an Email Header?

The header is a section of the email containing information such as sender,
recipient, and date. There are also components such as 'Return-Path', 'Reply-To', and 'Received'. 

What does the Email Header do?

--Allows you to identify the sender and recipient
--Spam Blocker
--Allows You to Track an Email's Route

Domain Key and Domain Key Identified Mail (DKIM) are email signatures that help 
email service providers identify and authenticate your emails, similar to SPF signatures.

The Message-ID header is a unique combination of letters and numbers that identifies each email. 
No two emails will have the same Message ID.

Multipurpose Internet Mail Extensions (MIME) is an Internet coding standard. 
It converts non-text content, such as images, videos, and other attachments, 
into text so that non-text content can be attached to an email and sent via 
SMTP (Simple Mail Transfer Protocol).

The X-Spam Status shows you the spam score of an email message.
```
### If we wanted to respond to this email, what would be the recipient's address?
> **ANSWER: info@letsdefend.io**
### What year was the email sent?
> **ANSWER: 2022**
### What is the Message-ID? (without > < )
> **ANSWER: 74bda5edf824cea8aad36e707.675c34a61f.20220321204512.a02caaccf3.a268ce5a@mail41.suw13.rsgsv.net**

## 4) Email Header Analysis
Here are the key questions we need to answer when checking headings during a Phishing analysis:

* Was the email sent from the correct SMTP server?
* Are the data "From" and "Return-Path / Reply-To" the same?


### Are the sender’s address and the address in the “Reply-To” area different?
> **ANSWER: y**
### If I want to reply to this email, which address will it be sent to?
> **ANSWER: mrs.dara@daum.net**
### What IP address was the email sent from?
> **ANSWER: 222.227.81.181**


## 5) Static Analysis

```
By querying VirusTotal for web addresses in emails, you can find out if the 
antivirus engines detect the web address as harmful. If someone else has already 
analyzed the same address/file in VirusTotal, VirusTotal will not analyze it 
from scratch, it will show you the old analysis result. This feature can be 
considered both an advantage and a disadvantage.
```
> **ANSWER: CHECK**

## 6) Additional Techniques
> **ANSWER: CHECK**

## 7) Quiz
### At what stage of the Cyber Kill Chain are phishing attacks carried out?
> **ANSWER: Delivery**
### Where should you check to see if an email is spoofed?
> **ANSWER: Email header**
### Which protocol does not help you to determine whether an e-mail has been spoofed or not?
> **ANSWER: UDP**
### What does SMTP stand for?
> **ANSWER: Simple Mail Transfer Protocol**
### Which of these are not part of the header of an e-mail?
> **ANSWER: Check**
### Which of the following cannot be achieved through a phishing attack?
> **ANSWER: SQL injection**
# 100% CORRECT