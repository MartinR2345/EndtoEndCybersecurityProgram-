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

<strong>Why This Step Was Important</strong><br>
The objective for this step is to determine what can go wrong for this organization and why.

<p align="center">
 <strong>Step Five: Perform The Risk Assessment & Create Risk Register Table </strong> <br/>

<p align="center">
  <img src="https://i.imgur.com/gYxr9Ip.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

I performed a risk assessment that measures risk using likelihood and impact scores to determine how severe a risk is depending on where the risk score lands on the rating scale. This allows me to evaluate how serious the identified cybersecurity risks are and how much damage it could cause to this fintech payment-processing environment. </br>

I document the results in the risk register (spreadsheet) below. This spreadsheet highlights the assessed risks, threats, vulnerabilities, risk scenarios, likelihood, impact score, the overall risk score and risk level. 

<p align="center">
  <img src="https://i.imgur.com/0zSZO1q.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Was Important</strong><br>
The objective for this step is to assess risk or analyze risk by identifying, evaluating, and tracking potential threats and opportunities for this fictional organization.

<p align="center">
 <strong>Step Six: Identify Existing Security Controls </strong> <br/>

I identify the existing security controls to highlight the current safeguards already protecting the environment.
The question I asked myself: </br>

“What is AI Driven currently doing to reduce those vulnerabilities?”</br>

The first thing I did was review my vulnerabilities from Step 4 and give it context/meaning in the spreadsheet below: 
<p align="center">
  <img src="https://i.imgur.com/3hXTLgl.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

I wrote out the existing controls below:

<strong>Existing Controls</strong>
<strong>MFA (partial adoption)</strong> - AI Driven currently uses multi-factor authentication on some employee and administrative accounts to provide an additional layer of login security and reduce unauthorized access risks.. This helps AI Driven add an extra layer of login security to reduce unauthorized access if passwords are stolen. This greatly reduces account compromise and unauthorized access.

<strong>AWS IAM </strong> - AI Driven uses AWS IAM to manage user permissions and restrict access to cloud systems and sensitive resources based on user roles. This helps AI Driven control user permissions and limit access to AWS systems and sensitive cloud resources based on user roles and responsibilities. 

<strong>Endpoint protection or Antivirus</strong> - AI Driven currently performs basic logging and monitoring activities to help identify suspicious system activity and support incident investigations. This helps AI Driven detect and block malware, ransomware and malicious files on employee laptops

<strong>Basic logging & Monitoring</strong> - This helps AI Driven identify suspicious activity and supports incident detection and investigations.

<strong>Security Awareness Training</strong> - AI Driven provides basic cybersecurity awareness training to help employees identify phishing emails, suspicious links, and social engineering attacks. This helps AI Driven employees identify suspicious emails, avoid malicious links and report phishing attempts. This also reduces credential theft.

<strong>Data Encryption</strong> - AI Driven uses data encryption to protect PCI payment card data, customer information, and sensitive business data from unauthorized access and disclosure.

<strong>Backup & Recovery Procedures</strong> - AI Driven maintains backup and recovery procedures to restore critical systems and recover data following ransomware attacks, system failures, or other disruptive incidents.

<strong>Why This Step Was Important</strong><br>
The objective for this step is to document all cybersecurity controls that currently exist.

<p align="center">
 <strong>Step Seven: Conduct the Current State Cybersecurity Assessment (Baseline Assessment) </strong> <br/>

This is where I changed viewpoints. From step 1 to step 6, I basically created everything I needed for this fictional company to exist. Now in step 7, the idea is:

 <strong>"Pretend I was hired as a cybersecurity consultant. I interviewed executives, IT administrators, developers, HR, and other stakeholders. I reviewed documentation, asked questions, and took notes. Those notes became my Current State Assessment.”</strong>

This baseline is not the future state but it represents what currently exists, what currently works, what is missing, and what is partially implemented. 


During the assessment I evaluated:
<ol>
 <li><strong>Organizational Governance</strong></li>
</ol>

<p align="center">
  <img src="https://i.imgur.com/feweEvd.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/ZHg4YCQ.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/83L9RGD.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/k1LZwNW.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/Tie3qUL.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/ERhODd0.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/jwqXRAR.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/LQkc1WU.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/L7uyTLD.png" height="50%" width="60%" alt="SaveRecords"/>
</p>


<p align="center">
  <img src="https://i.imgur.com/flEobhx.png" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Was Important</strong><br>
The objective for this step is to gather evidence by interviewing stakeholders, reviewing policies and procedures, observing existing controls and documenting the current state.

<p align="center">
 <strong>Step Eight: Perform the NIST CSF Control Assessment (PASS / FAIL) </strong> <br/>

I perform the NIST CSF Control Assessment to evaluate each NIST CSF control by comparing it against the Current State Baseline. 

<p align="center">
  <img src="" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Was Important</strong><br>
The objective for this step is to compare the evidence from Step 8 against the NIST CSF and determine whether each control passes or fails and record comments explaining the decision.

<p align="center">
 <strong>Step Nine: Develop a Risk-Based Cybersecurity Improvement Plan </strong> <br/>

<p align="center">
  <img src="" height="50%" width="60%" alt="SaveRecords"/>
</p>

 <strong>Why This Step Was Important</strong><br>
The objective for this step is to analyze every failed control and recommend practical improvements to close the gaps as well as prioritize recommendations based on business risk and PCI-DSS requirements.

   
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
