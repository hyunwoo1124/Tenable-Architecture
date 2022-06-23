# Tenable Architecture Diagram
Tenable Architecture for Vulnerability management


![Tenable Architecture](https://user-images.githubusercontent.com/31784131/175198631-1b1dff9b-f316-4669-a929-92f7c42a1590.png)

# Summary
Tenable is a great vulnerability management solution. Tenable provides visibility of your environment for on-prem and cloud applications. In this project, I demonstrate Tenable Architecture in 3 different Cloud instances, Tenable.io and nessus scanner that reports to central security center in a single-pane of glass.

# 3 Offices and Tenable.io
Each office has multiple VLANs for different departments such as HR, Marketing, Engineering, IT and more. Nessus scanner for Office x can scan endpoints for malware/compliance/vulnerability and report it to Nessus Scanner. Nessus Scanner then reports to the Security Center. Tenable.io nessus agent scans endpoints with credential by default which provides greater visibility of the endpoints. The scans then report it to the security center.

# AWS, AWS Gov, and Azure
Instances in any of the cloud can be reported to the security center for vulnerability management. Commercial clouds has Tenable integration that can be seamlessly connected to the security center. Government cloud is a manual process. Some applications are recommended to only download nessus agents only.

# Definitions
Tenable.io Nessus Agent - Agent based vulnerability management that scans endpoints as credential scan. Great for web apps and endpoints

Nessus Scanner - Scanner that's deployed onto on-prem and or cloud server that scans different subnets. It can report it to the main Tenable.sc (Security Center).

Tenable Core + Tenable.sc - Tenable Core is a RHEL based OS system specifically for Tenable. It provides network statistics, CPU usage, and more that also host Tenable.sc (Security Center). Tenable.sc is a main single-pane of glass dashboard that provide great telemetry and vulnerability management tools for remote offices and cloud enviornment.

