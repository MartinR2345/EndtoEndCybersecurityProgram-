<h1>End-To-End Cybersecurity Program</h1>

<h2>Video Demonstration</h2>
 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
This repository demonstrates how I conducted a full cybersecurity program assessment for a fictional company called AI Driven using the the NIST Cybersecurity Framework. The goal is to transform this messy, insecure organization (AI Driven) into a structured, risk-aware cybersecurity program aligned with the NIST Cybersecurity Framework.
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

 <strong>Why This Step Was Important</strong><br>
This creates the organizational context, operational environment, business risk profile and compliance landscape. The objective is to understand the business.

<p align="center">
 <strong>Step Two: Define Systems, Users, Devices & Sensitive Data </strong> <br/>

The current “Systems” (within scope) for AI Driven are:
<ol>
 <li><strong>AWS cloud infrastructure</strong> - This connects to web application, database, backups and hosts the fintech platform and cloud services </li>
 <li><strong>Payment Processing Web Application</strong> - This connects to customers, APIs, databases and basically customer-facing payment portal </li>
 <li><strong>Transaction Database</strong> - This stores PCI payment data and transaction history </li>
 <li><strong>Employee Endpoint Devices</strong> - This is used by employees, administrators and developers for daily operations</li>
 <li><strong>Email & Collaboration Systems </strong> - This is for internal communication and business operations</li>
 <li><strong>Backup & Recovery Systems</strong> - This supports disaster recovery and business continuity.</li>
</ol>

I chose these systems because all these systems allow AI Driven to process payments, store transaction data, support customers, communicate internally and maintain business operations. This is everything the company uses to run its business operations.

The current “Users” (users interacting with the environment) in Scope for AI Driven are:
<ol>
 <li><strong>Employees</strong> - The primary role is to handle daily business operations. </li>
 <li><strong>Developers</strong> - The primary role is to build and maintain applications. </li>
 <li><strong>IT Administrators</strong> - The primary role is to manage cloud and infrastructure and systems </li>
 <li><strong>Customers</strong> - The primary role is to use payment platform services. </li>
</ol>

The current “Devices (devices supporting operations)” in Scope for AI Driven are:

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

 <strong>Why This Step Was Important</strong><br>
The objective for this step is to identify what is being assessed. This scope is extremely important because it establishes what systems are being protected, what data is included, what users are in scope, what assets are assessed, what controls apply and what auditors review.  Without a defined scope, risks become unclear and controls become inconsistent.

<p align="center">
 <strong>Step Three: Identify Critical Business Assets </strong> <br/>

<p align="center">
  <img src="https://i.imgur.com/jTujD3c.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

I identified five critical business assets for AI Driven by asking myself these two question:
<ol>
 <li>What assets are most important to protect?</li>
 <li>How badly would the company suffer if this system failed or got compromised?</li>
 <li>Would it cause financial loss, downtime, compliance violations, customer impact or reputational damage?</li>
</ol>

The five <strong>“Critical Business Assets”</strong> I chose were: 
<ol>
 <li><strong>Payment Processing Web Application</strong> - It is responsible for processing financial transactions and supporting business revenue generation. It's a customer-facing platform. </li>
 <li><strong>Transaction database</strong> - This stores sensitive PCI payment card data, customer information, and financial transaction records</li> 
 <li><strong>AWS Cloud Infrastructure </strong> - This hosts cloud services, applications, databases, and supporting business operations</li>
 <li><strong>Backup and Recovery Systems</strong> - This supports disaster recovery, ransomware recovery, and operational resilience
<li><strong>Authentication systems</strong> - This controls user authentication, access permissions, and protection against unauthorized access</li>
</ol>

These five assets are the systems most likely to be targeted by attackers, impact business operations if compromised and trigger compliance violations as well as require the strongest security controls. 

<strong>Why This Step Was Important</strong><br>
The objective for this step is to determine what must be protected. 

<p align="center">
 <strong>Step Four: Identify Threats, Vulnerabilities, Risk Scenarios </strong> <br/>

<p align="center">
  <img src="https://i.imgur.com/GQ9zwoX.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

I gave this fictional company (AI Driven) <strong>three threats</strong>, <strong>seven vulnerabilities/existing security weaknesses</strong>. I then connected my threats and vulnerabilities together to show how they go hand in hand and this connection helped me create <strong>five risk scenarios</strong> for my five critical business assets.

<strong>THREATS</strong> (Something that could potentially cause harm to company) </br>
<ol>
 <li><strong>Phishing Attacks</strong> - Attackers attempt to trick users into revealing credentials or downloading malicious content</li>
  <li><strong>Cloud Based Attacks</strong> - Attackers target weaknesses within the AWS cloud environment</li>
  <li><strong>Web Applications Attacks</strong> - Attackers exploit weaknesses within the payment processing application</li>
</ol>

<strong>VULNERABILITIES</strong> (A weakness that attackers can exploit) </br>
<ol>
 <li><strong>Weak MFA Adoption</strong> - Multi-factor authentication is not consistently enforced across systems. Multi-factor authentication is not fully enforced across all employee, administrative, and cloud accounts, increasing the risk of unauthorized access if credentials are compromised.</li>
  <li><strong>Cloud Misconfiguration</strong> - Improper AWS security settings or exposed cloud resources. Misconfigured AWS cloud resources and security settings could expose sensitive systems and data to unauthorized access.</li>
  <li><strong>Unpatched Systems</strong> - Systems and applications are not updated regularly with security patches. Some systems and applications may not receive timely security updates or patches, increasing exposure to known vulnerabilities and exploits.</li>
  <li><strong>Limited Security Monitoring</strong> - Limited centralized monitoring and threat detection capabilities. AI Driven currently has limited centralized logging and monitoring capabilities, which may delay the detection and response to suspicious activity or security incidents.</li>
  <li><strong>Weak Security Awareness Training</strong> - Employees receive limited cybersecurity and phishing awareness training. Employees may not receive frequent or advanced cybersecurity awareness training, increasing the likelihood of successful phishing and social engineering attacks. </li>
 <li><strong>Insufficient Data Encryption</strong> - Sensitive data may not be consistently encrypted across all systems, databases, storage locations, or transmission channels. This could increase the risk of unauthorized disclosure of PCI payment card data and customer information if systems are compromised. </li>
 <li><strong>Inadequate Backup and Recovery Testing</strong> - Although backup processes exist, backups may not be regularly tested or validated to ensure successful recovery during a cyber incident, ransomware attack, or system outage. This could increase recovery time and operational disruption. </li>
</ol>

<strong>THE CONNECTION BETWEEN THREATS & VULNERABILITY TOGEHTER </strong> </br>
<p align="center">
  <img src="https://i.imgur.com/p675uSV.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<strong>RISK SCENARIOS</strong> (Describe realistic events that could occur) </br>
   
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
