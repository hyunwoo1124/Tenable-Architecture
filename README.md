# Tenable-Architecture
Tenable Architecture for Vulnerability management


![Tenable Architecture](https://user-images.githubusercontent.com/31784131/175198631-1b1dff9b-f316-4669-a929-92f7c42a1590.png)

# Summary
Tenable is a great vulnerability management solution. Tenable provides visibility of your environment for on-prem and cloud applications. In this project, I demonstrate Tenable Architecture in 3 different Cloud instances, Tenable.io and nessus scanner that reports to central security center in a single-pane of glass.

# 3 Offices and Tenable.io
Each office has multiple VLANs for different departments such as HR, Marketing, Engineering, IT and more. Nessus scanner for Office x can scan endpoints for malware/compliance/vulnerability and report it to Nessus Scanner. Nessus Scanner then reports to the Security Center. Tenable.io nessus agent scans endpoints with credential by default which provides greater visibility of the endpoints. The scans then report it to the security center.
