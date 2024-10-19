<h1> File Integrity Monitor </h1>

 ### [Post Demonstration](https://medium.com/@lmb.walid/integriy-monitor-file-fim-and-hashing-algorithms-6eda8b77dce6)

 <h2>Description</h2>
This project is a simple PowerShell-based File Integrity Monitoring (FIM) system that helps detect unauthorized changes to files. It uses hashing algorithms (SHA-512) to compare current file states against a saved baseline. If any file is created, modified, or deleted, the system alerts the user with real-time notifications.
<br/>
<br/>
<br/>

<p align="center">
System Diagram<br/>
<img src="https://github.com/user-attachments/assets/adc32864-4c7a-464b-819d-4996147bc74f" height="60%" width="60%" alt="System Diagram"/>
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Windows 11</b>

<h2>Program walk-through:</h2>

<h4>Path A: Collect a New Baseline</h4>

- calculates the current hash values for the target files and stores them in a file called <i>baseline.txt</i>


<p align="center">
Hash values for the target files <br/>
<img src="https://github.com/user-attachments/assets/a7d9387f-1d95-4ec0-a256-f17688f3ccd1" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br/>


<h4>Path B: Monitor Files Using the Saved Baseline</h4>


<p align="center">
Monitoring Files<br/>
<img src="https://github.com/user-attachments/assets/36aafa2e-661f-45cc-ab0e-bc51e11d2001" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br/>
 


 
