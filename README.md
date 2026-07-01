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

 I created a company called AI Driven. It is a fictional startup Financial Technology SaaS company that provides cloud-hosted payment processing services and PCI-DSS compliance requirements.  It is an AWS cloud environment and has minimal security team maturity.
  <ul>
  <img src="https://i.imgur.com/Uh3mIGu.png" height="80%" width="80%" alt="SaveRecords"/></li>
 </ul>

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
Employees - The primary role is to handle daily business operations
Developers - The primary role is to build and maintain applications
IT Administrators - The primary role is to manage cloud and infrastructure and systems 
Customers - The primary role is to use payment platform services.




   
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
