<h1>Mini Compliance Program</h1>

<h2>Video Demonstration</h2>
 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
This repository demonstrates how I built a mini compliance program by selecting a framework (ISO 27001 Annex A) and creating a fictional healthcare clinic called SaveRecords that stores electronic patient records.
<br />

<h2>Framework Used</h2>

<ul> <li>ISO 27001 Annex A</li>

</ul>

<h2>Task To Complete</h2>

<ul>
  <li>Choose a fictional company (for example, a SaaS startup or healthcare clinic) and define its scope: assets, systems, users, and data types.</li>
  <li>Download the ISO 27001 Annex A control list or NIST 800-53 catalog to use as your baseline requirements.</li>
  <li>Create a spreadsheet with columns such as Control ID, Requirement, Current Status, Owner, and Needed Actions.</li>
 <li>Select at least 15–20 controls that apply to your environment and document whether they are implemented, partially implemented, or missing.</li>
 <li>Write a brief one-page “Compliance Program Overview” describing your chosen scope, goals, and current level of maturity.</li>
 <li>Highlight 3–5 gaps and propose realistic remediation steps that an organization could take to improve compliance readiness.</li>
 <li>Store all evidence (matrix, notes, document drafts) as part of your growing portfolio.</li>
</ul>

<h2>Program walk-through:</h2>

<p align="center">
  <strong>Phase One: Define The Fictional Organization</strong> <br/>

 I needed a clear story for the compliance environment so first, I identify from personal experience of the type of jobs I worked. Healthcare came to mind. Healthcare is naturally high compliance relevance (HIPAA, ISO 27001, etc). With healthcare comes electronic records and data types like PII and PHI. 
  <ul>
  <li><strong>Compliance Environment Story:</strong> A healthcare clinic called SaveRecords that stores electronic patient records and protects confidential data (PII/PHI)</li>
 </ul>
     
<p align="center">
 <strong>Phase Two: Define Assets, Systems, Users & Data Types with ChatGPT Assistance</strong> <br/>

 Once I created the compliance enviroment story, I ask ChatGPT to list the assets, systems, users, and data types that fits to this compliance environment story. 
 <ul>
  <li><strong>Assets:</strong> EMR application (custom web app), Cloud database (AWS), Staff laptops/workstations, Internet routers/firewalls, Patient data repository (contains PII and PHI)</li>
  <li><strong>Systems:</strong> AWS (hosting and data storage), EMR platform (used by staff), Internal email and file-sharing tools</li>
  <li><strong>Users:</strong> Doctors, Admin Staff, Nurses, IT Support</li>
  <li><strong>Data Types:</strong> Personally Identifiable Information (PII), Protected Health Information (PHI)</li>
 </ul>

This gives me a nice scoping statement I can plug into my ISO 27001 documents later.  It defines what's in scope (systems, assets, data) and who interacts with them.

<p align="center">
 <strong>Phase Three: Write out the Scope Summary </strong> <br/>

 I basically reviewed Phase Two and wrote a quick scope summary around this fictional company (SaveRecords Health Clinic)

<strong>Scope Summary:</strong>
SaveRecords Health Clinic operates an internal patient management system where doctors, nurses, and admin staff access patient records stored in a secure cloud environment. The scope of this compliance program includs the clinics information systems, electronic medical record (EMR) platforms, staff laptops and patient data store in the cloud.
 
<p align="center">
 <strong>Phase Four: Choose A Framework </strong> <br/>

 ISO 27001 Annex A Framework Information: <br>
https://www.isms.online/iso-27001/annex-a-2022/
 
 I chose (ISO 27001 Annex A framework) for my healthcare clinic scenario because it's globally recognized, risk based, and structured for exactly what SaveRecords needs which is protecting PII and PHI in a systematic way. 

<p align="center">
 <strong>Phase Five: Pick 20 Controls from ISO 27001 Framework </strong> <br/>

 ISO 27001 Annex A Framework Information: <br>
https://www.isms.online/iso-27001/annex-a-2022/
 
ISO 27001 (Annex A) has 93 controls group under four themes:
<ul>
 <li>Organization (A.5 - A.8 - 37 Controls): Policies, procedures, and governance.</li>
 <li>People (A.6 - 8 Controls): Background checks, training, and awareness.</li>
 <li>Physical (A.7 - 14 Controls): Secure areas, equipment, and surveilance.</li>
 <li>Technological (A.8 - 34 Controls): Network security, encryption, and access management.</li>
</ul>
  
For a small healthcare clinic like 'SaveRecords', I picked 20 controls that make the most sense for my compliance environment and put it on a google sheets. 

<p align="center">
 <img src="https://i.imgur.com/JubBivS.png" height="80%" width="80%" alt="twentyControls"/>
<br />

<p align="center">
 <strong>Phase Five:  Build a Mini Control Matrix in Excel or Google Sheets. </strong> <br/>

I create a google sheet and named it "Mini Contract Matrix" then added columns to this sheet and 20 controls as well.

<strong>Columns to include:</strong> <br>
| Control ID | Requirement | Current Status | Owner | Needed Actions | <br>

Note to self: <br>
<strong>Requirements</strong> - What does this control provides? <br>
<strong>Current Status</strong> = a quick self-assessment of your maturity (Implemented / Partially / Missing). <br>
<strong>Owner</strong> = who is the person or role accountable for that control's success (not necessarily the one doing the work) (like Clinic Director, IT Manager, HR Manager, Compliance Officer,  etc.). <br>
<strong>Needed Actions / Remediation Notes</strong> = realistic next steps that would show progress toward full compliance. <br>

<p align="center">
 <img src="https://i.imgur.com/cfgsLp1.png" height="80%" width="80%" alt="twentyControls"/>

 <p align="center">
 <strong>Phase Six: Add the Requirements, Owners On The Sheet With ChatGPT Assistance </strong> <br/>

 I use ChatGPT to assist with adding the requirements, and owners to this google sheet. I rewrote every line and use ChatGPT as a mentor, not a quick fix. How I use ChatGPT is, I ask it to give me the answer for one control then I do my own research and write out the next 19 controls then I asks ChatGPT to review each control I wrote and provide feedback on how it can be better.

<p align="center">
 <img src="https://i.imgur.com/SjMBfwo.png" height="80%" width="80%" alt="twentyControls"/>

<p align="center">
 <img src="https://i.imgur.com/rgbixPl.png" height="80%" width="80%" alt="twentyControls"/>

<p align="center">
 <img src="https://i.imgur.com/mCCk63T.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <strong>Phase Six: Assign a Maturity Rating To 20 Controls Current Status</strong> <br/>

I created a google sheet and named it "3-Level Maturity Scale 2026". 

<p align="center">
 <img src="https://i.imgur.com/Dbt4OFA.png" height="80%" width="80%" alt="twentyControls"/> <br>

 When reviewing each control, I ask myself these quick checks: <br>
 Do we have a written policy or procedure for this? <br>
 If Yes, then choose either Partially or Fully Implemented<br>
 If No, then choose Missing

 Is the process consistently followed by all staff? <br>
 If Yes, then choose Implemented <br>
 If No, then choose Partially <br>

 Is there documentation or evidence (logs, reports, training records)? <br>
 If Yes, then choose Implemented <br>
 If No, then choose either Partially or Missing <br>

 Has management reviewed or approved it recently? <br>
 If Yes, then choose Implemented <br>
 If No, then choose either Partially or Missing <br>

 Basically, I thought of this as a mini risk assessment. Instead of picking randomly, I remind myself that this should be logical so for each control, I assigned either implemented (fully operational), partially implemented (informal or incomplete), missing (no process yet) for the Current Status.

 <p align="center">
 <img src="https://i.imgur.com/umCvw0w.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <img src="https://i.imgur.com/2yFDYR8.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <img src="https://i.imgur.com/vWutFSE.png" height="80%" width="80%" alt="twentyControls"/> <br>

Note to Self:
I also used ChatGPT to review all of my 20 control Current Status for feedback...

  <p align="center">
 <strong>Phase Seven: Needed Actions: Write a short, specific, and actionable</strong> <br/>

   The “Needed Actions” column is where my matrix really comes alive. This is where I shift from identifying the state of compliance to proposing realistic next steps for SaveRecords Health Clinic. <br>
  
   The “Needed Actions” column answers one simple question: <br>
   “What’s the next step required to bring this control to full compliance?”

 <p align="center">
 <img src="https://i.imgur.com/5avzD8p.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <img src="https://i.imgur.com/dgb9rDl.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <img src="https://i.imgur.com/BYXD9mZ.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <strong>Phase Eight: Compliance Program Overview</strong> <br/>

   The “Compliance Program Overview” is the final piece that ties this mini compliance program together. The goal was to tell the story of SaveRecords Health Clinic's security posture, what framework it follows, where it stands now, and what it plans to improve. <br>

 <p align="center">
 <img src="https://i.imgur.com/I4UYhwM.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <img src="https://i.imgur.com/sXgI7na.png" height="80%" width="80%" alt="twentyControls"/> <br>

  <p align="center">
 <img src="https://i.imgur.com/eJ5OZvk.png" height="80%" width="80%" alt="twentyControls"/> <br>

   
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
