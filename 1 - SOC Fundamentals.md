# LECTURE1: SOC Fundamentals

## 1) Introduction to SOC
Welcome to the first step of your career as a SOC analyst. In this first lesson, the structure
of SOC and SOC tools will be explained. The lesson will also discuss why a SOC analyst
needs these SOC (Security Operations Center) tools and how to use them effectively.

What will you learn in this course?

* The structure of a SOC

* Operation of a SOC

* SOC Tools/Products

* How a SOC Analyst should use his tools

* Common mistakes made by SOC Analysts

By covering the above topics with a hands-on approach in the LetsDefend SOC
environment, you will be able to improve your understanding and progress quickly.

If You Want To Become a SOC Analyst

If becoming a SOC Analyst is your career goal, we recommend you focus on SOC tools
such as SIEM, Log Management, and EDR, and take notes.

After you complete this course, you can move on to more technically advanced courses.
However, you should start with this course first.

If You Are a SOC Analyst

If you are a SOC Analyst and are here to accelerate your professional development, there
are sections labeled "Quick Tips" just for you, as well as numerous examples of mistakes
that are made. You can study these topics and focus on applying best practices to avoid
making mistakes.

Last but not least

To get the most out of this training, you must complete it. The content is comprehensive
and all topics are linked. It may be difficult to complete all the content in one day, but if you
divide it into daily and weekly periods, you can complete the program successfully.

Answer: CHECK

## 2) SOC Types and Roles
What is a SOC?

A Security Operation Center (SOC) is a facility where the information security team
continuously monitors and analyzes the security of an organization. The primary purpose of
the SOC team is to detect, analyze, and respond to cybersecurity incidents using
technology, people, and processes.

Types of SOC Models

Depending on your security needs and budget, there are several types of SOCs:

![Image 1](SOC/Assets/1 - SOC Fundamentals/1.png)

In-house SOC

This team is formed when an organization builds its cybersecurity team. Organizations
considering an internal SOC should have a budget to support its continuity.

Virtual SOC

This type of SOC team does not have a permanent facility and often works remotely in
various locations.

Co-Managed SOC

The Co-Managed SOC consists of internal SOC staff working with an external Managed
Security Service Provider (MSSP). Coordination is key in this type of model.

Command SOC

This SOC team oversees smaller SOCs across a large region. Organizations using this
model include large telecommunications providers and defense agencies.

People, Process, and Technology

Building a successful SOC requires serious coordination. Most importantly, there should
be a strong relationship between people, processes, and technology.

Simply put, we will discuss the people, processes, and technologies required for SOC.

![Image 2](SOC/Assets/1 - SOC Fundamentals/2.png)

People

A strong SOC team requires highly trained personnel who are familiar with security alerts
and attack scenarios. Because attack types are constantly changing, you need team
members who can easily adapt to new attack types and are willing to conduct research.

Processes

To further develop your SOC structure, you need to align it with many different types of
security requirements, such as NIST, PCI, and HIPAA. All processes require extreme
standardization of actions to ensure nothing is left out.

Technology

The team needs to have different products for many tasks, such as penetration testing,
detection, prevention, and analysis, and they need to follow the market and technology
closely to find the best solution for the organization. Sometimes the best product on the
market may not be the best product for your team. Remember to consider other factors
such as the organization's budget.

SOC Roles

SOC Analyst

This role can be categorized as Level 1, 2, and 3 according to the SOC structure. A security
analyst classifies the alert, looks for the cause, and advises on remediation.

Incident Responder

An Incident Response Officer is an individual responsible for threat detection. This role
performs the initial assessment of security breaches.

Threat Hunter

A Threat Hunter is a cybersecurity professional who proactively seeks out and investigates
potential threats and vulnerabilities within an organization's network or system. They use a
combination of manual and automated techniques to detect, isolate, and mitigate
advanced persistent threats (APTs) and other sophisticated attacks that may evade
traditional security measures. Threat hunters typically have a deep understanding of the
organization's IT infrastructure and security posture, as well as knowledge of emerging

threats and attack tactics. They aim to find and eliminate threats before they can damage
or disrupt the business.

Security Engineer

Security engineers are responsible for maintaining the security infrastructure of Security
Information and Event Management (SIEM) solutions and security operations center (SOC)
products. For example, a security engineer builds the connection between SIEM and
Security Orchestration, Automation, and Response (SOAR) products.

SOC Manager

A SOC manager takes on management responsibilities such as budgeting, strategizing,
managing staff, and coordinating operations. They deal with operational rather than
technical issues.

> **ANSWER: CHECK**

## 3) SOC Analyst and Their Responsibilities
In this section, we will discuss what a SOC Analyst is, where they fit into the SOC team,
and the general responsibilities of the role. It is important to review these sections carefully
before learning about the technical side of the role. In this way, aspiring SOC Analyst
candidates can get an idea of what their future career might look like.

A SOC Analyst is the first person to investigate threats to a system. If the situation demands
it, they escalate incidents to their supervisors so they can mitigate threats. The SOC
Analyst plays an important role on the SOC team because they are the first person to
respond to a threat.

The Advantages of Being a SOC Analyst

There are many various techniques for attack vectors and malicious software and they
increase more and more every day. As an analyst you will get greater enjoyment from

![Image 3](SOC/Assets/1 - SOC Fundamentals/3.png)

investigating these varying types of incidents. Even though the operating systems, security
products, etc. that you use will be the same the job will feel less monotonous because you
will be analyzing different incidents. Also, you may not encounter such techniques (not
every week or every day).

A Day in the Life of a SOC Analyst

Throughout the day, a SOC analyst typically reviews alerts in the SIEM and determines
which ones are real threats. To reach a conclusion, they use various security and
protection products such as Endpoint Detection and Response (EDR), Log Management,
and SOAR. We will explain in detail why and how these products are used later in the
training program.

To be a successful SOC analyst who is not dependent on security products and can
correctly analyze SIEM alerts, you must have the following skills and abilities.

Operating Systems

To determine what is abnormal in a system, you first need to know what is accepted as
normal. For example, there are many services within the Windows operating system, and it
is difficult to know which ones are suspicious without knowing which ones are or could be
considered normal Windows services. Therefore, you should be familiar with how
Windows/Linux operating systems work.

Network

First and foremost, in this role, you will be dealing with a lot of malicious IPs and URLs, so
you need to confirm that there are no devices on the network trying to connect to those
addresses. Once you accomplish that, it will set the direction of the analysis.

This step is a bit more complicated because you may have to find a potential data leak on
the network. To perform all of these functions, you need to understand the basics of
networking.

Malware Analysis

When dealing with most threats, you are likely to encounter some type of malicious
software. To understand the real purpose of these malicious programs (they sometimes
display different behaviors to fool analysts), you need to have malware analysis skills.

It is important to at least determine what the command-and-control center of the
malicious file is and whether or not there is a device communicating with that address.

In general, we have discussed what a SOC analyst is, what the responsibilities of the role
are, and what skills a SOC Analyst needs to have. As the course progresses, it will also
cover technical areas, starting with SIEM.

> **ANSWER: CHECK**

## 4) SIEM and Analyst Relationship
This lesson discusses what SIEM is, why it is used in a SOC, and how SIEM relates to the
SOC analyst.

What is SIEM?

SIEM is a security solution that combines security information and event management,
which involves real-time logging of events in an environment. The ultimate purpose of event
logging is to detect security threats.

Overall, SIEM products have a lot of features. The ones that interest us most as SOC
analysts are those that collect and filter data and provide alerts for suspicious events.

Example alert: If someone on a Windows operating system tries to enter 20 incorrect
passwords in 10 seconds, this is suspicious activity. It is unlikely that someone who has
forgotten their password would try to re-enter it that many times in such a short period of
time. So we create a SIEM rule/filter to detect such activity that exceeds the threshold.
Based on this SIEM rule, an alert will be generated when such a situation occurs.

![Image 4](SOC/Assets/1 - SOC Fundamentals/4.png)

Some popular SIEM solutions: IBM QRadar, ArcSight ESM, FortiSIEM, Splunk, etc. To get a
better picture, you can visit the “Monitoring” page on LetsDefend.

Relationship Between a SOC Analyst and SIEM

Although SIEM solutions have many features, SOC analysts typically only track alerts.
There are other groups/people responsible for developing configurations and rule
correlations.

As mentioned above, alerts are generated from data that passes through filters. Alerts are
first analyzed by a SOC analyst. This is where a SOC analyst's job in the security operations
center begins. In essence, they have to determine whether the generated alert is a real
threat or a false alert.

For a better understanding, let's go back to the "Monitoring" page; as you can see below,
there are various alerts on the SIEM interface. A SOC analyst should analyze the details
related to these alerts with the help of other SOC products (such as EDR, Log
Management, Threat Intelligence Feed, etc.) and ultimately determine whether they are
real threats or not.

You can view newly created alerts in the "Main Channel" and think of this channel as a
shared channel. Your teammates are not visible in this simulation, but in a real work
scenario, your teammates will be able to see this panel. After you select the alert you want
to work on, click the Take Ownership button in the Action area to take ownership of the
alert and direct it to the Investigation Channel. This way, your teammates can see which
alert you are actively working on. At the same time, this will help them see which alerts you
are already working on so they can select other alerts. This way, your team can quickly
review all alerts.

When you click on the alert, you can see the details of the alert. This allows you to gather
the information (hostname, IP address, file hash information, etc.) required to investigate.

Quick Tip

Note that from time to time, false alerts may be generated in the SIEM. A good SOC analyst
would be able to identify such situations and provide feedback to the team, thereby
contributing to the efficiency of the SOC team.

Example:

Let's say that an SIEM team has put together a rule set that generates alerts for URL
addresses that have the word "union" in them and is trying to detect SQL injections.

A user did a search using "https://www.google.com/search?q=sql+union+usage", and an
alert was created in the SIEM, it looks like there is no obvious threat. The alert was
generated because the keyword "union" was included in the URL. These types of anomalies
can be shared with the SIEM team to optimize the alerting process.

Final Words

So far, we have covered what SIEM is, how it helps SOC analysts, and how it should be
used. Later in our course, we will discuss how to analyze an alert created in the SIEM.

When you close an alert, which channel(tab on the monitoring page) can you access it
from?

> **ANSWER: Closed Alerts**

## 5) Log Management
As a SOC Analyst, you will perform a lot of log analysis. For this reason, it is important to be
familiar with "Log Management" systems/solutions. It doesn't matter what product you
use, it's about knowing what to look for and where to look for it.

The remainder of this lesson discusses how "Log Management" solutions can be used
effectively by SOC analysts.

What is Log Management?

![Image 7](SOC/Assets/1 - SOC Fundamentals/7.png)

As the name implies, Log Management provides access to all logs in an environment (web
logs, OS logs, firewall, proxy, EDR, etc.) and allows you to manage them in one place. This
increases efficiency and saves time.

If you can't access the logs from one place, then the same request (e.g., the goal is to
determine all users on letsdefend.io) would have to be sent to different devices. This would
increase your margin for error and the amount of time you would need to spend.

If you go to the “Log Management” page in LetsDefend, you will see various log sources
such as Proxy, Exchange, and Firewall listed as “Type”. This means that all these log
sources have been collected in one place and log output from sources like Proxy, FW, etc.
can be seen with just one query.

Purpose of Log Management

SOC analysts typically rely on Log Management to determine if there is any communication
with a particular address and to view the details of that communication. Let's say you
came across a piece of malware and after running it, you found that it was communicating
with and executing commands from the "letsdefend.io" address. In this situation, the
command&control center is "letsdefend.io", you can search for "letsdefend.io" in your
company's log management to see if any devices have attempted to communicate with the
command&control center.

This leaves us with a second situation: You see a SIEM alert indicating that a
LetsDefendHost device on your network is leaking data to IP address 122[.]194[.]229[.]59.
You have conducted an investigation, isolated the device from the network, performed the
necessary processes, and now you are in control. But there's still something you haven't
addressed: are there any other devices sending data to the suspicious IP address
(122[.]194[.]229[.]59)? The alert may have only included LetsDefendHost, but you should
still search for the suspicious address in Log Management to see if there is anything the
system may not have detected and try to find any connections.

What source IP address entered the URL 'https://github.com/apache/flink/compare'?

> **ANSWER: 172.16.17.54**

What is the type of log that has a destination port number of 52567 and a source IP address
of 8.8.8.8?

> **ANSWER: DNS**

## 6) EDR - Endpoint Detection and Response
A SOC analyst must spend a significant amount of time using EDR when performing
analysis on an endpoint device. The following sections discuss why EDR is beneficial to
SOC analysts and how to use it effectively.

What is EDR?

Endpoint Detection and Response (EDR), also known as Endpoint Threat Detection and
Response (ETDR), is an integrated endpoint security solution that combines continuous,
real-time monitoring and collection of endpoint data with rules-based automated response
and analysis capabilities. (Definition source: mcafee.com)

Analysis with EDR

Some EDR solutions commonly used in the workplace: CarbonBlack, SentinelOne, and
FireEye HX.

To understand what you can do with EDR as an analyst, let's take a look at "Endpoint
Security" on LetsDefend.

As you can see in the image, the accessible endpoint devices are listed on the left. You can
search for endpoints in the search bar, or if there is an IOC (an IP address, file hash,
process name, etc.), we can perform a search across all hosts.

The right side displays general information about the device and shows sections such as
Browser History, Network Connections, and Process List.

Live Investigation

Next, you can click the Connect button and access the machine itself to continue the
analysis.

Containment

You need to isolate a hacked machine from the network. There are two important reasons
for doing this: to prevent the attacker from connecting to the internal network and moving
around the internal network.

Therefore, the device should be isolated from the internal and external networks until the
vulnerabilities are repaired and the device is ready for use. You can ensure isolation by
using the containment feature of EDR solutions. This feature allows the selected device to

communicate solely with the EDR center. This means that even though the device is
isolated from the network, you can continue your analysis.

![Image 12](SOC/Assets/1 - SOC Fundamentals/12.png)

Quick Tip

If you have any type of IOC, such as a file hash, file name, etc., you can perform a search in
EDR across all hosts and see if there is a match. For example, let's say you are certain that
a device has been hacked and you have obtained a file with an MD5 hash of
"ac596d282e2f9b1501d66fce5a451f00". You can search for this hash value in EDR and
determine whether this file exists or is being executed on other devices. This will help you
understand who has been affected by this attack.

Conclusion

We covered the basics of EDR, which you will use just as often as Log Management. In the
past, we have seen analysts fail to use EDR solutions effectively, so spending some time on
this topic will put you one step ahead of the crowd.

Please remember to go to " Endpoint Security ” to practice, and then review the alerts on
the “Monitoring” page.

In the next section, we will discuss how to speed up the analysis process with SOAR.

What is the hostname of the device where the “nmap” file with a hash value of
“83e0cfc95de1153d405e839e53d408f5” is executed?

> **ANSWER: EricProd**

A "Ps1.hta" file was executed on a device with the hostname "Roberto". What is the
complete CMD command?

> **ANSWER: C:/Windows/System32/mshta.exe C:/Users/roberto/Desktop/Ps1.hta**

## 7) SOAR (Security Orchestration Automation and Response)
SOAR stands for Security Orchestration Automation and Response. It enables security
products and tools in an environment to work together, streamlining the tasks of SOC team
members. For example, it will automatically search VirusTotal for the source IP of a SIEM
alert, reducing the workload of the SOC analyst.

Some SOAR products commonly used in the industry:

* Splunk Phantom

* IBM Resilient

* Logsign

* Demisto

The image below shows what can be achieved with a SOAR solution.

![Image 13](SOC/Assets/1 - SOC Fundamentals/13.png)

image: hawk-eye.io

The benefits of SOAR and how you can effectively use SOAR as a SOC analyst will be the
focus of the rest of this lesson.

Saves You Time

SOAR saves time with workflows that automate processes. Some common workflows are:

* IP address reputation control

* Hash query

* Scanning an acquired file in a sandbox environment

Centralization (A single platform for everything you need)

It allows you to use different security tools in your environment (sandbox, log management,
3rd party tools, etc.) by providing an all-in-one software. These tools are integrated into the
SOAR solution and can be used on the same platform.

image: splunk.com

Playbooks

You can easily investigate SIEM alerts using playbooks created for different scenarios
within SOAR. Even if you don't know or remember all the procedures, you can perform an
analysis by following the steps outlined in the playbooks

In addition, these playbooks help ensure that the entire SOC team is on the same page
when performing their analysis. For example, all team members need to check IP
reputation, so if one team member is not checking it and the others are, this is an
undesirable situation. We can avoid this situation by adding this step to the playbook.

LetsDefend and SOAR

You can think of "Case Management" as the same as SOAR. On the SIEM (monitoring) page,
you can open tickets for the cases you created. When you look at the page, the first thing
you see is a list of open and closed cases.

If you click on any open case, you will see an automatically assigned playbook. You can
investigate the associated SIEM (monitoring) alert following this playbook.

So far, we have covered what a SOAR solution is, how it is used in a SOC environment, and
how it benefits SOC analysts in general. In the next lesson, we will explore threat
intelligence and how it relates to a SOC analyst.

ANSWER : CHECK

## 8) Threat Intelligence Feed
A SOC team should be immediately aware of the latest threats and take the necessary
precautions. To meet this need, threat intelligence feeds are created. As a SOC analyst,
you can use these feeds to guide your investigations.

A Threat Intelligence Feed is data (such as malware hashes, C2 (Command&Control)
domain/IP addresses etc.) provided by a third party company.

Looking at LetsDefend's Threat Intel page, you can see many types of data (hash, IP, etc.)

The data here consists of artifacts from previous malicious activity. It could be the hash of
malware or the IP address of a command and control center. As a SOC analyst, you need to
search threat intelligence feeds to determine if a hash file at hand has ever been used in a
malicious scenario in the past.

Here are some free and popular sources you can use:

* VirusTotal

* Talos Intelligence

Important points to highlight:

If data you run through feeds does not show up

Let's say you ran a hash of an .exe in VirusTotal and in the past you didn't find anything
suspicious about it. In this case, you should not just assume that the file is clean, that
would be a mistake. A SOC analyst should carefully perform the necessary file analysis
(static/dynamic).

We shouldn’t forget that IP addresses can change hands.

For example, let's say an attacker created a server on AWS (Amazon Web Services) and
used it as a command and control center. Then various threat intelligence feeds listed that
IP address as a malicious address.

2 months later, the attacker shut down the server and someone else moved their personal
blog to that server. This doesn't mean that people who visited the blog were exposed to
malicious content. The fact that this IP address has been used for malicious purposes in
the past does not mean that it contains malicious content.

> **ANSWER: AbuseCH**

## 9) Common Mistakes made by SOC Analysts
Like everyone else, SOC analysts can make mistakes. In this section, we will discuss
common mistakes made by SOC analysts and how to avoid making them yourself.

* Over-reliance on VirusTotal Results

* Hasty Analysis of Malware in a Sandbox

* Inadequate Log Analysis

* Overlooking VirusTotal Dates

It is recommended that you review this lesson after you have completed the previous
lessons in this course.

Over-reliance on VirusTotal Results

Sometimes we can rely on the result displayed on VirusTotal’s green screen after analyzing
a file’s URL and seeing that the address is harmless. However, there is a new malicious
software developed using an AV (AntiVirus) bypass technique that may not be detected by
VT (VirusTotal). For this reason, we should accept VirusTotal as a supporting tool and
perform our analyses with this in mind.

Here’s a detailed blog post on the subject for further reading: VirusTotal is not an Incident
Responder

Hasty Analysis of Malware in a Sandbox

A 3-4 minute analysis in a sandbox environment may not always yield accurate results.
Here are the reasons why:

Malware might be able to detect a sandbox environment and will not activate itself.

Malware may not become active for 10 to 15 minutes after the operation is performed.

For this reason, the duration of the analysis should be kept as long as possible and it
should take place in a real environment, if possible.

Inadequate Log Analysis

Occasionally we see that some log analysis is not performed properly. For example, let's
say that a piece of malware has been detected on a machine with the hostname
"LetsDefend", and that malware is secretly sending data to the address "letsdefend.io". As
a SOC analyst, you should use Log Management solutions to determine if any other device
is also attempting to connect to this address.

Overlooking VirusTotal Dates

If the search you performed in VirusTotal has already been queried, a result from the cache
will be displayed. For example: We searched the address "letsdefend.io" in VirusTotal and
the result is shown below.

An attacker could simply search a clean URL on VirusTotal and replace it with malicious
content. This is why you should not just look at the search cache, but conduct a new
search.

Conclusion

This lesson covered common mistakes made by SOC analysts and how to avoid them.
Don't forget to revisit this section from time to time to refresh your memory.

> **ANSWER: CHECK**
