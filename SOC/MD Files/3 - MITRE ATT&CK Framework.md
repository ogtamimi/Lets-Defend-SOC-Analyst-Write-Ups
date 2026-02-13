# LECTURE3: MITRE ATT&CK Framework

## 1) Introduction
> **ANSWER: CHECK**
## 2) Introduction to MITRE

```
What is MITRE ATT&CK Framework?
MITRE ATT&CK that stands for Adversarial Tactics, Techniques, 
and Common Knowledge is the framework of a knowledge database that was introduced by MITRE in 2013 and has been continuously 
developed and expanded along with the technology. It is possible to analyze cyber attacks systematically through the MITRE ATT&CK framework. 
Cyber attacks can be divided into certain stages and the methods used in each stage can be analyzed in depth and used in studies related to cyber security. 
The MITRE ATT&CK Framework is an essential resource for each 
and every employee in the cybersecurity industry.
```

### In what year was the MITRE founded?
> **ANSWER: 1958**
### In what year was MITRE ATT&CK Framework started to be developed?
> **ANSWER: 2013**

## 3) Matrix

```
What is MITRE ATT&CK Matrix?
MITRE ATT&CK Matrix is a visualization method used to classify and see attack methods of
cyber attackers. 
Matrices can be customized for almost any subject and turned into useful visuals. MITRE has created MITRE ATT&CK
matrices to visualize the details of attacker behavior using the matrices.

3 different matrices have been created within
the MITRE ATT&CK Framework according to the platform types:

1-Enterprise Matrix : Enterprise matrix is the first matrix created by MITRE. 
There are more digital systems included in this matrix and are 
more common than those that are included in other matrices, 
so there are a lot more information in this matrix than other matrices. 
Enterprise matrix is mainly used to understand the cyber attacks on large organizations.

There are 7 sub-matrices under the Enterprise Matrix:
--PRE
--Windows
--macOS
--Linux
--Cloud
--Network
--Containers

2-Mobile Matrix : The mobile matrix is the one that was prepared for mobile devices and
contains information about the cyber security of mobile devices. 
This matrix can be used to ensure the security of individual and corporate mobile devices.
Comparing the Enterprise Matrix, it contains less information:

Mobile Matrix has 2 sub-matrices:
--Android
--iOS

3-ICS (Industrial Control Systems) Matrix : The ICS Matrix is the one that contains the information collected for the cyber security of devices in the industrial control systems. This matrix can be used to provide cyber security and analyses of an ICS.

```
### What are the images depicting tactics and techniques in the MITRE ATT&CK Framework called?
> **ANSWER: Matrix**
### What is the matrix of information about the cybersecurity of Windows, Linux, macOS, Azure AD and Office 365 platforms?
> **ANSWER: Enterprise**
### What is the matrix that contains the information about the cyber security of Android and iOS platforms?
> **ANSWER: mobile**

## 4) Tactics

Tactic expresses the purpose of the cyber attacker and the reason for his action. 
Tactics are one of the most important MITRE ATT&CK Framework components 
used to group cyber attacker behaviors and see the attack steps. 
Tactics are in the top row of the matrix.

#### Enterprise Tactics
There are 14 tactics in the Enterprise matrix as in the list below:
* Reconnaissance
* Resource Development
* Initial Access
* Execution
* Persistence
* Privilege Escalation
* Defense Evasion
* Credential Access
* Discovery
* Lateral Movement
* Collection
* Command and Control
* Exfiltration
* Impact

#### Mobile Tactics
There are 14 tactics in the Mobile matrix as in the list below:
* Initial Access
* Execution
* Persistence
* Privilege Escalation
* Defense Evasion
* Credential Access
* Discovery
* Lateral Movement
* Collection
* Command and Control
* Exfiltration
* Impact
* Network Effects
* Remote Service Effects

#### ICS Tactics
There are 12 tactics in the ICS matrix as in the list below:
* Initial Access
* Execution
* Persistence
* Privilege Escalation
* Evasion
* Discovery
* Lateral Movement
* Collection
* Command and Control
* Inhibit Response Function
* Impair Process Control
* Impact

### What is the ID of the "Lateral Movement" tactic in the Enterprise matrix?
> **ANSWER: TA0008**
### When was the "Persistence" tactic in the mobile matrix created?
> **ANSWER: 17 October 2018**
### Which tactic in the Enterprise, Mobile, and ICS matrices is used to obtain higher-level permissions on target systems or networks?
> **ANSWER: Privilege Escalation**


## 5) Techniques and Sub-Techniques

```
The techniques and sub-techniques, on the other hand show the methods used by the attacker to achieve his goal and how he conducted the attack exactly. Each technique/sub-technique is included within the matrix depending on a particular tactic. As an example, some of the techniques on the enterprise matrix are shown in the image below:

What is Procedure?
The procedure consists of usage examples of techniques/sub-techniques. 
It simply shows which tool/software was utilized during the 
implementation of the technique. In other words, it is the 
explanation of the practical information on the use of the technique.
```
### What is the name of the technique with the ID T1055 among the Enterprise techniques?
> **ANSWER: Process Injection**
### Among the Enterprise techniques, which platform is the technique with the ID T1112 for?
> **ANSWER: Windows**
### In the MITRE ATT&CK framework, which tactic does the 'Supply Chain Compromise' technique fall under?
> **ANSWER: Initial Access**

## 6) Mitigations
Mitigations refers to the measures and actions that can be taken in response to the techniques in the MITRE ATT&CK matrix. Each mitigation has a unique ID, name and description that provides clear understanding about them.

### What is the name of the mitigation with the ID M1032 among the Enterprise mitigations?
> **ANSWER: Multi-factor Authentication**
### What is the name of enterprise mitigation that recommends “digital signature verification should be implemented to prevent the untrusted codes from working on enterprise devices”?
> **ANSWER: Code Signing**

## 7) Groups
Advanced Persistent Threat (APT) Groups, are the hacker groups that may include many different people and groups that carry out cyber attacks in a targeted and systematic way, with governments support from time to time. APT groups may conduct cyber attacks with different motivations. For example, the group may have a specific mission, may be conducting their attacks for money, or may be foreign government supported and conduct their attacks to obtain their national ideals.

Within the MITRE ATT&CK Framework, information about APT groups is collected which helps identify which APT group is targeting which systems and which cyber attack techniques are being implemented. When all this information is gathered together and evaluated with the MITRE ATT&CK matrix, the attack map of the APT group can be revealed.
### What is the name of the software that is associated only with the "System Information Discovery" technique among the software utilized by the OilRig APT group?
> **ANSWER: systeminfo**
### What is the name of the APT group whose “Associated Groups” information includes the names “GOLD NIAGARA”, “ITG14” and “Carbon Spider”?
> **ANSWER: FIN7**

## 8) Software
In the software section of MITRE ATT&CK Framework, there are software used by APT groups.
Each software has a unique ID, name and description. For example, the below image shows the ID, Name and the Description of the software
### For which platform is the software named “Cryptoistic” utilized by “Lazarus Group” APT group meant for?
> **ANSWER: MacOS**
### What is the type of software named “Rotexy” for Android platforms?
> **ANSWER: Malware**
### What is the name of the APT group that utilizes the software named “PUNCHBUGGY” targeting POS networks?
> **ANSWER: FIN8**

## Quiz 
### What is the concept that expresses the motivation for the action of the cyber attacker within the MITRE ATT&CK Framework?
> **ANSWER: Tactic**
### What is the concept that explains how the cyber attacker performs his action within the MITRE ATT&CK Framework?
> **ANSWER: Technique**
### What is the concept that expresses the application examples of the method used by the cyber attacker within the MITRE ATT&CK Framework?
> **ANSWER: Procedure**
### Which of the following is an ID of a technique in the MITRE ATT&CK Framework?
> **ANSWER: T1426**
### Which of the following enterprise techniques belongs to a different tactic?
> **ANSWER: Exploit Public-Facing Application**
### In which matrix is the “Impair Process Control” tactic located?
> **ANSWER: ICS Matrix**
### What is the tool used for credential dumping specifically only for Linux systems by the “TeamTNT” APT group?
> **ANSWER: MimiPenguin**
