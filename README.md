<h1>End-To-End Cybersecurity Program</h1>

<h2>Video Demonstration</h2>
 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
This repository demonstrates how I conducted an end-to-end cybersecurity program assessment for a fictional FinTech SaaS startup called AI Driven. Acting as an external Cybersecurity/GRC Consultant, I established the organization's current cybersecurity baseline, performed a NIST Cybersecurity Framework (CSF) control assessment, identified security gaps, and developed a prioritized remediation roadmap to improve the organization's cybersecurity posture.
<br />

<h2>Framework Used</h2>

<ul> <li>NIST Cybersecurity Framework</li>

</ul>

<h2>Task To Complete</h2>

<ul>
 <li>Define the Fictional Company & Business Environment</li>
 <li>Define Systems, Users, Devices & Sensitive Data </li>
 <li>Identify Critical Business Assets</li>
 <li>Identify Threats, Vulnerabilities, Risk Scenarios </li>
 <li>Perform The Risk Assessment & Create Risk Register Table</li>
 <li>Identify Existing Security Controls</li>
 <li>Conduct the Current State Cybersecurity Assessment (Baseline Assessment)</li>
 <li>Perform the NIST CSF Control Assessment (PASS / FAIL)</li>
 <li>Develop a Risk-Based Cybersecurity Improvement Plan</li>
</ul>

<h2>Program walk-through:</h2>
<p align="center">
  <strong>Step One: Define the Fictional Company & Business Environment</strong> <br/>

 I created a fictional company called AI Driven that is a startup Financial technology SaaS company. This fictional organizaiton provides cloud-hosted payment processing services and PCI-DSS compliance requirements.  It is an AWS cloud environment and has minimal security team maturity.

<p align="center">
  <img src="https://i.imgur.com/Uh3mIGu.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Matters</strong><br>
The objective of Step 1 creates the organizational context, operational environment, business risk profile and compliance landscape. The objective is to understand the business.

<p align="center">
 <strong>Step Two: Define Systems, Users, Devices & Sensitive Data </strong> <br/>

I identified the “Systems” (within scope - that support the business). This included:
<ol>
 <li><strong>AWS cloud infrastructure</strong> - This connects to web application, database, backups and hosts the fintech platform and cloud services </li>
 <li><strong>Payment Processing Web Application</strong> - This connects to customers, APIs, databases and basically customer-facing payment portal </li>
 <li><strong>Transaction Database</strong> - This stores PCI payment data and transaction history </li>
 <li><strong>Employee Endpoint Devices</strong> - This is used by employees, administrators and developers for daily operations</li>
 <li><strong>Authentication systems</strong> - a digital bouncer. It verifies your identity—proving you are who you claim to be—before granting you access to an app, website, or device/li>
 <li><strong>Email</strong> - This is for internal communication and business operations</li>
 <li><strong>Backup Systems</strong> - This supports disaster recovery and business continuity.</li>
</ol>

I chose these systems because all these systems allow AI Driven to process payments, store transaction data, support customers, communicate internally and maintain business operations. This is everything the company uses to run its business operations.

I also identified the “Users" of the environment: 
<ol>
 <li><strong>Employees</strong> - The primary role is to handle daily business operations. </li>
 <li><strong>Developers</strong> - The primary role is to build and maintain applications. </li>
 <li><strong>IT Administrators</strong> - The primary role is to manage cloud and infrastructure and systems </li>
 <li><strong>Customers</strong> - The primary role is to use payment platform services. </li>
</ol>

I identified the “Devices" (devices supporting operations):

<ol>
 <li><strong>Employee Laptops</strong> - This connects employees to email systems, cloud environments, internal applications and payment systems. Devices like windows laptops, macbooks.  </li>
 <li><strong>AWS Cloud Servers</strong> - They may host payment applications, APIs, databases and backend services. Such as EC2 instances, virtual servers. </li>
</ol>

Sensitive data like: 
<ol>
 <li><strong>PCI Payment Card Data</strong> - This is regulated financial data. If a company stores or processes credit card numbers, debit card information, CVV codes, expiration dates, it cannot protect that data however it wants. Instead, it must follow specific security requirements created by the payment card industry. </li>
 <li><strong>Customer PII</strong> - Examples like customers name, emails, phone numbers, and billing address </li>
 <li><strong>Financial Transaction Records</strong> - Examples like payment history, invoices, merchant activity</li>
 <li><strong>Authentication Data</strong> - Examples like passwords, MFA tokens, API keys, session tokens </li>
</ol>

 <strong>Why This Step Matters</strong><br>
The objective of Step 2 is to identify what is being assessed. This scope is extremely important because it establishes what systems are being protected, what data is included, what users are in scope, what assets are assessed, what controls apply and what auditors review.  Without a defined scope, risks become unclear and controls become inconsistent.

<p align="center">
 <strong>Step Three: Identify Critical Business Assets </strong> <br/>

<p align="center">
  <img src="https://i.imgur.com/jTujD3c.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

Once I understood the environment, I asked myself these two question:
<ol>
 <li>What assets are most important to protect?</li>
 <li>How badly would the company suffer if this system failed or got compromised? Would it cause financial loss, downtime, compliance violations, customer impact or reputational damage?</li>
</ol>

The five <strong>“Critical Business Assets”</strong> I chose were: 
<ol>
 <li><strong>Payment Processing Web Application</strong></li>
 <li><strong>Transaction database</strong></li> 
 <li><strong>AWS Cloud Infrastructure </strong></li>
 <li><strong>Authentication systems</strong></li>
 <li><strong>Backup and Recovery Systems</strong></li>
</ol>

These assets became the primary focus of the risk assessment.

<strong>Why This Step Matters</strong><br>
The objective of Step 3 is to determine what must be protected. These five assets are the systems most likely to be targeted by attackers, impact business operations if compromised and trigger compliance violations as well as require the strongest security controls. 

<p align="center">
 <strong>Step Four: Identify Threats, Vulnerabilities, Risk Scenarios </strong> <br/>

<p align="center">
  <img src="https://i.imgur.com/GQ9zwoX.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

I identified the major cybersecurity <strong>threats</strong> (Something that could potentially cause harm to company) facing the organizaiton. </br>

Examples included:
<ol>
 <li><strong>Phishing Attacks</strong> - Attackers attempt to trick users into revealing credentials or downloading malicious content</li>
  <li><strong>Cloud Attacks</strong> - Attackers target weaknesses within the AWS cloud environment</li>
  <li><strong>Web Applications Attacks</strong> - Attackers exploit weaknesses within the payment processing application</li>
</ol>

I also identified <strong>vulnerabilities</strong> (A weakness that attackers can exploit) such as:  </br>
<ol>
 <li><strong>Weak MFA Adoption</strong> - Multi-factor authentication is not consistently enforced across systems. Multi-factor authentication is not fully enforced across all employee, administrative, and cloud accounts, increasing the risk of unauthorized access if credentials are compromised.</li>
  <li><strong>Cloud Misconfigurations</strong> - Improper AWS security settings or exposed cloud resources. Misconfigured AWS cloud resources and security settings could expose sensitive systems and data to unauthorized access.</li>
  <li><strong>Limited Security Monitoring</strong> - Limited centralized monitoring and threat detection capabilities. AI Driven currently has limited centralized logging and monitoring capabilities, which may delay the detection and response to suspicious activity or security incidents.</li>
  <li><strong>Unpatched Systems</strong> - Systems and applications are not updated regularly with security patches. Some systems and applications may not receive timely security updates or patches, increasing exposure to known vulnerabilities and exploits.</li>
  <li><strong>Weak Security Awareness Training</strong> - Employees receive limited cybersecurity and phishing awareness training. Employees may not receive frequent or advanced cybersecurity awareness training, increasing the likelihood of successful phishing and social engineering attacks. </li>
</ol>

I then combined the threats and vulnerabilities into realistic risk scenarios that described how an attacker could exploit these weaknessess below: </br>
<strong>THE CONNECTION BETWEEN THREATS & VULNERABILITY TOGEHTER </strong> </br>
<p align="center">
  <img src="https://i.imgur.com/p675uSV.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<strong>RISK SCENARIOS</strong> (Describe realistic events that could occur) </br>

<strong>Asset 1 — Payment Processing Web Application</strong> </br>
An attacker exploits a vulnerability in the payment processing web application because security patches are not applied promptly, resulting in unauthorized access, payment fraud, or service disruption. </br>

<strong>Asset 2 — Transaction Database</strong> </br>
An attacker gains unauthorized access to the transaction database because of cloud misconfigurations, exposing PCI payment card data, customer information, and financial records.

<strong>Asset 3 — AWS Cloud Infrastructure</strong> </br>
An attacker gains access to AWS resources because cloud security settings are misconfigured, resulting in data exposure or disruption of critical business services.

<strong>Asset 4 — Backup & Recovery Systems</strong> </br>
An attacker compromises backup and recovery systems through a phishing attack because employees are not adequately trained, preventing the organization from restoring systems after a ransomware attack.

<strong>Asset 5 — Authentication Systems</strong> </br>
An attacker successfully phishes an employee and gains access to authentication systems because MFA is not fully enforced, allowing unauthorized access to employee, developer, and administrator accounts.

<strong>Why This Step Matters</strong><br>
The objective of Step 4 is to determine what can go wrong for this organization and why.

<p align="center">
 <strong>Step Five: Perform The Risk Assessment & Create Risk Register Table </strong> <br/>

<p align="center">
  <img src="https://i.imgur.com/gYxr9Ip.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

After identifying the risks, I assessed each one by evaluating it's likelihood and business impact to determine how severe the risk is depending on where the risk score lands on the rating scale. </br>

I then documented these risks in a risk register (this spreadsheet) and assigned risk ratings to help prioritize which issues required the most immediate attention. This helped demonstrate a risk-based approach to cybersecurity rather than treating every issue as equally important.

<p align="center">
  <img src="https://i.imgur.com/0zSZO1q.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Matters</strong><br>
The objective of Step 5 is to assess risk or analyze risk by identifying, evaluating, and tracking potential threats and opportunities for this fictional organization.

<p align="center">
 <strong>Step Six: Identify Existing Security Controls </strong> <br/>

I identified the security controls that were already in place 

The first thing I did was review my vulnerabilities from Step 4 and give it context/meaning in the spreadsheet below: 
<p align="center">
  <img src="https://i.imgur.com/3hXTLgl.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

AI Driven had implemented several underlying controls, including:

<strong>Existing Controls</strong>
<ol>
 <li><strong>AWS IAM </strong> - AI Driven uses AWS IAM to manage user permissions and restrict access to cloud systems and sensitive resources based on user roles. This helps AI Driven control user permissions and limit access to AWS systems and sensitive cloud resources based on user roles and responsibilities. </li>
 <li><strong>Partial Multi-Factor Authentication</strong> - AI Driven currently uses multi-factor authentication on some employee and administrative accounts to provide an additional layer of login security and reduce unauthorized access risks.. This helps AI Driven add an extra layer of login security to reduce unauthorized access if passwords are stolen. This greatly reduces account compromise and unauthorized access.</li>
 <li><strong>Endpoint protection</strong> - AI Driven currently performs basic logging and monitoring activities to help identify suspicious system activity and support incident investigations. This helps AI Driven detect and block malware, ransomware and malicious files on employee laptops</li>
 <li><strong>Basic logging & Monitoring</strong> - This helps AI Driven identify suspicious activity and supports incident detection and investigations.</li>
 <li><strong>Data Encryption</strong> - AI Driven uses data encryption to protect PCI payment card data, customer information, and sensitive business data from unauthorized access and disclosure.</li>
 <li><strong>Backup & Recovery Procedures</strong> - AI Driven maintains backup and recovery procedures to restore critical systems and recover data following ransomware attacks, system failures, or other disruptive incidents.</li>
 <li><strong>Security Awareness Training</strong> - AI Driven provides basic cybersecurity awareness training to help employees identify phishing emails, suspicious links, and social engineering attacks. This helps AI Driven employees identify suspicious emails, avoid malicious links and report phishing attempts. This also reduces credential theft.</li>
</ol>

<strong>Why This Step Matters</strong><br>
The objective of Step 6 is to document all cybersecurity controls that currently exist.

<p align="center">
 <strong>Step Seven: Conduct the Current State Cybersecurity Assessment (Baseline Assessment) </strong> <br/>

I assumed the role of an external Cybersecurity Consultant hired by AI Driven.
I conducted interviews with key stakeholders, including executive leadership, the IT Manager, Cloud Administrator, HR, and other personnel.  I also reveiwed available documentation and documented my observations about the organizations's current cybersecurity environment. 

This baseline represents what currently exists, what currently works, what is missing, and what is partially implemented. These observations became the evidence used during the next step.

<p align="center">
  <img src="https://i.imgur.com/A6iN4pC.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/5rMqwXr.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/wCfuGhe.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/y8X1pYm.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/mqpHEv3.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/tHqW9l3.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/9LpUhX2.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Matters</strong></br>
The objective of Step 7 is to gather evidence by interviewing stakeholders, reviewing policies and procedures, observing existing controls and documenting the current state and use this information for Step 8.

<p align="center">
 <strong>Step Eight: Perform the NIST CSF Control Assessment (PASS / FAIL) </strong> <br/>

Using the baseline assessment from Step 7, I evaluated AI Driven against the NIST Cybersecurity framework. </br>
For each control, I determined whether the organization passed or failed based on the evidence collected during Step 7. This helped me identfiy control gaps across governance, identity management, monitoring, incident response, disaster recovery, and many other security domains.

<strong>IDENTIFY</strong>
<p align="center">
  <img src="https://i.imgur.com/I2mZAM3.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/X2tUboa.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/uRyuRCe.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/hgpTHRf.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/rgXnZjt.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<strong>PROTECT</strong>
<p align="center">
  <img src="https://i.imgur.com/2K9AiBE.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/V8ZkP6x.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/ZY5OgKp.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/HVBDm5m.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/mC2uf3p.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/FYXrydL.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/vcOYXPt.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<strong>DETECT</strong>
<p align="center">
  <img src="https://i.imgur.com/XHU78Rr.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/9r3uU98.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/aHK2Qhp.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<strong>RESPOND</strong>
<p align="center">
  <img src="https://i.imgur.com/zfoG67h.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/FUqhroQ.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/XbqybQr.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/GbIMZWr.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/lCSa64f.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<strong>RECOVER</strong>
<p align="center">
  <img src="https://i.imgur.com/ZIwjrlZ.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/RJhVXQg.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/7rqv9Vr.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Matters</strong><br>
The objective of Step 8 is to compare the evidence from Step 7 against the NIST CSF and determine whether each control passes or fails and record comments explaining the decision.

<p align="center">
 <strong>Step Nine: Develop Recommendations Based On The Assessment Findings</strong> <br/>
Finally, I developed a prioritized set of recommendations for AI Driven. <br/>
<p align="center">
  <img src="https://i.imgur.com/8XWq2uB.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/T8LWSr6.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/U4yaCCg.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Matters</strong><br>
The objective of Step 9 is to provide management a set of cybersecurity recommendations for AI Driven based on the gaps identified during the Current State Cybersecurity Baseline Assessment and the NIST CSF Control Assessment. The recommendations are intended to help AI Driven strengthen its security controls, address identified risks, improve compliance with PCI-DSS requirements, and enhance its overall cybersecurity maturity.

   
<h2>Lessons Learned:</h2>
<ul>
 <li>Understanding how compliance frameworks are structured</li>
 <li>Learning how to map controls to business processes</li>
 <li>Identifying gaps and building remediation plans</li>
 <li>Documenting compliance maturity in a clear, structured format</li>
</ul>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
