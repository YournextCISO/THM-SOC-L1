# Friday Overtime!!

![image](https://github.com/user-attachments/assets/0b318ac5-53d9-452b-8fc3-d0b4bfb98c67)

## Scenario
It's a Friday evening at PandaProbe Intelligence when a notification appears on your CTI platform. While most are already looking forward to the weekend, you realise you must pull overtime because SwiftSpend Finance has opened a new ticket, raising concerns about potential malware threats. The finance company, known for its meticulous security measures, stumbled upon something suspicious and wanted immediate expert analysis.

As the only remaining CTI Analyst on shift at PandaProbe Intelligence, you quickly took charge of the situation, realising the gravity of a potential breach at a financial institution. The ticket contained multiple file attachments, presumed to be malware samples.

With a deep breath, a focused mind, and the longing desire to go home, you began the process of:

Downloading the malware samples provided in the ticket, ensuring they were contained in a secure environment.
Running the samples through preliminary automated malware analysis tools to get a quick overview.
Deep diving into a manual analysis, understanding the malware's behaviour, and identifying its communication patterns.
Correlating findings with global threat intelligence databases to identify known signatures or behaviours.
Compiling a comprehensive report with mitigation and recovery steps, ensuring SwiftSpend Finance could swiftly address potential threats.

### Log into the CLI platform:
![image](https://github.com/user-attachments/assets/8fe62352-6dec-4284-bf1a-75b8d05dca56)



## Task 1
Who shared the Malware samples ? .
Take a look at the bottom of the ticket generated to find out.
![image](https://github.com/user-attachments/assets/b46b0e6e-bba8-4b84-aa80-efa2b1ebbf3c)

## Task 2
What is the SHA1 hash of the file "pRsm.dll" inside samples.zip?

Here we will use the CLI to extract and check the hash of the pRsm.dll file and run the commands ;unzip samples.zip
sha1sum pRsm.dll.
![image](https://github.com/user-attachments/assets/19d944eb-3526-4fd1-b598-4b9836904d68)

 - Ans : 9d1ecbbe8637fed0d89fca1af35ea821277ad2e8


# Task 3
Which malware framework utilizes these DLLs as add-on modules?

Hint: Google 
![image](https://github.com/user-attachments/assets/e25ae5ed-10ca-4fc7-9856-43be30fb1108)


 - Ans : MgBot

# Task 4
Which MITRE ATT&CK Technique is linked to using pRsm.dll in this malware framework?

![image](https://github.com/user-attachments/assets/ee5c0a86-38d3-4c90-b9b5-c6ae312acb5d)

 - Ans: T1123

## Task 5
What is the CyberChef defanged URL of the malicious download location first seen on 2020-11-02?

Locate the link and head over to cyberchef to defang
![image](https://github.com/user-attachments/assets/d89371f6-808b-46f7-8ba7-883609970460)

 - Ans : hxxp[://]update[.]browser[.]qq[.]com/qmbs/QQ/QQUrlMgr_QQ88_4296.exe

 ## Task 6
 What is the CyberChef defanged IP address of the C&C server first detected on 2020-09-14 using these modules?

![image](https://github.com/user-attachments/assets/159600f0-7bb5-47df-b09b-6568563c0387)

Defang using cyberchef
- Ans: 122[.]10[.]90[.]12

## Tsask 7
What is the SHA1 hash of the spyagent family spyware hosted on the same IP targeting Android devices on November 16, 2022?

Look up the IP on VirusTotal and check Relations. Search with the defanged IP .

![image](https://github.com/user-attachments/assets/92c74a49-ddfe-440f-bdf0-481f36380068)


We can verify if thats the correct hash we are looking for by clicking on it and it will give us more details :

![image](https://github.com/user-attachments/assets/5b3e6ad7-765c-4780-866c-76907bd9020f)

Now go under Details: ![image](https://github.com/user-attachments/assets/f0489d74-376f-41ef-b7b8-1a86e55cb7d6)




and there we have it. 

Success

 - Ans : 1c1fe906e822012f6235fcc53f601d006d15d7be



