# Microsoft Defender for Endpoint curated list of resources for DFIR

<p align="center">
  <img src="https://images2.imgbox.com/94/d2/6Jd7QaSP_o.jpg">
</p>

Hey, thank you stopping by! Well, being here means that you are either familiar with the discipline of Digital Forensics & Incident Reponse (DFIR) or you are interested in beginning to explore DFIR tools and techniques. The common denominator, no matter what your sense is around DFIR, is that you are using Microsoft Defender for Endpoint (MDE) and the wider Microsoft Azure and Microsoft 365 Defender environments. I hope you will enjoy the following resources which come from my notes and relevant research and testing I have done. Do you have any other resources that fit here? Drop me a line at any of my mediums [here](https://www.michalos.net/about/) or pull the repo and push your request to review it.

If you find this repo useful, don't forget to ⭐ it!

#### Table of Contents
- [Mitigate threats using Microsoft Defender for Endpoint](#mitigate-threats-using-microsoft-defender-for-endpoint)
- [Remote collection of Windows Forensic Artifacts using KAPE and MDE](#remote-collection-of-windows-forensic-artifacts-using-kape-and-mde)
- [@BertJanCyber Incident Response guide](#@bertjancyber-incident-response-guide)
- [THOR-Cloud forensic scanning through MDE](#thor-cloud-forensic-scanning-through-mde)
- [HUNTERS Human-Friendly Guide for Incident Response & Threat Hunting](#hunters-human-friendly-guide-for-incident-response-and-threat-hunting)
- [Microsoft Defender For Endpoint Live Response Script Sources](#microsoft-defender-for-endpoint-live-response-script-sources)
- [MGinsu: A tool for repackaging large collections to traverse Windows Defender Live Response](#ginsu:-a-tool-for-repackaging-large-collections-to-traverse-windows-defender-live-response)

---

### Mitigate threats using Microsoft Defender for Endpoint

What better way to begin the resource list other than Microsoft Learn itself? MDE supports a lot of functionalities including artifact collection, containment, live response, advanced hunting and others which help analysts and investigators unfold alerts and incidents.

 - [Mitigate threats using Microsoft Defender for Endpoint](https://learn.microsoft.com/en-us/training/paths/sc-200-mitigate-threats-using-microsoft-defender-for-endpoint/)

---

### Remote collection of Windows Forensic Artifacts using KAPE and MDE

KAPE (Kroll Artifact Parser and Extractor) is a powerful DFIR tool by Eric Zimmerman that primarily collects and processes collected files. [@DFIRanjith](https://twitter.com/DFIRanjith) and [Krzysztof Miodoński](https://www.linkedin.com/in/krzysztof-miodonski/) have built and published guides on how to deploy KAPE through MDE live response and collect forensic artefacts.

 - [Remote collection of Windows Forensic Artifacts using KAPE and MDE](https://medium.com/@DFIRanjith/remote-collection-of-windows-forensic-artifacts-using-kape-and-microsoft-defender-for-endpoint-f7d3a857e2e0)
 - [Collaboration between KAPE and MDE at the service of the SOC](https://www.linkedin.com/pulse/collaboration-between-kape-microsoft-defender-service-miodo%C5%84ski-ip2vf)

---

### @BertJanCyber Incident Response guide

Bert-Jan ([@BertJanCyber](https://twitter.com/BertJanCyber)), a fellow community contributor has prepared a detailed and comprehensive guide on how to accommodate Microsoft technologies available including KQL queries and Live Response in order to practice the DFIR discipline.

 - [Incident Response Part 1: IR on Microsoft Security Incidents (KQL edition)](https://kqlquery.com/posts/kql-incident-response/)
 - [Incident Response Part 2: What about the other logs?](https://kqlquery.com/posts/kql-incident-response-everything-else/)
 - [Incident Response Part 3: Leveraging Live Response](https://kqlquery.com/posts/leveraging-live-response/)

---

### THOR-Cloud forensic scanning through MDE

THOR-Cloud allows live compromise assessment scans for YARA, Sigma and IOCs on endpoints through MDE. THOR-Cloud Lite comes with a free plan as well.

 - [THOR Cloud Lite Release Session](https://www.youtube.com/watch?v=ApeXFnFkKZg)
 - [THOR Cloud Lite - Microsoft Defender ATP Integration](https://www.youtube.com/watch?v=RubV7Cr1_FA)

---

### HUNTERS Human-Friendly Guide for Incident Response and Threat Hunting

HUNTERS, an advanced platform that leverages SIEM to help SOC teams, provides highly technical blogs around Microsoft Security. They started unfolding a series of blogs about IR and Threat hunting that really go deep into platform, differentiating sources, user's permissions etc.

 - [The Human-Friendly Guide: Incident Response & Threat Hunting in Microsoft Azure, Part 1](https://www.hunters.security/en/blog/human-friendly-guide-incident-response-microsoft-and-threat-hunting-azure-1?s=03)

---

### Microsoft Defender For Endpoint Live Response Script Sources

Repositories hosting Powershell script samples for "Live Response" that can be leveraged in your Microsoft Defender For Endpoint Environment.

 - [Powershell Digital Forensics & Incident Response (DFIR)](https://github.com/Bert-JanP/Incident-Response-Powershell)
 - [Microsoft Defender Advanced Threat Protection LiveResponse](https://github.com/YongRhee-MDE/LiveResponse)

---

### Ginsu: A tool for repackaging large collections to traverse Windows Defender Live Response

This script uses 7zip (7za.exe) to compress a specified folder and then splits the resulting archive into sections of 3GB or less. It will work (and was designed for) files larger than 3GB. Windows Defender Live Response currently only supports pulling back files of 3GB or less via the console.

 - [Ginsu: A tool for repackaging large collections to traverse Windows Defender Live Response](https://bakerstreetforensics.com/2023/11/16/ginsu-a-tool-for-repackaging-large-collections-to-traverse-windows-defender-live-response/)
 - [Ginsu Github Repo](https://github.com/dwmetz/Ginsu)

---

Last update: 24/01/2024
