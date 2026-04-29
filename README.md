# Development of Custom Open Source Intelligent Application

**Type:** Group Assignment
**Institution:** Illinois Institute of Technology

## Overview

This is a group project in which we designed, developed, and implemented a custom open source intelligent application in Python. The application is a Phishing Detection Tool with a graphical user interface (GUI) built using Tkinter. It retrieves and processes data from four distinct threat intelligence APIs to analyze URLs and IP addresses for phishing risk, and generates a detailed analysis report for each input.

The project included a full project management lifecycle alongside the technical development, covering planning, risk management, earned value tracking, and data analysis of results.

## Application Details

The tool accepts a URL or IP address as input. It routes the input through the appropriate APIs based on whether the input is a URL or IP address, aggregates the results, determines a risk verdict, and saves a report to local history.

**APIs Integrated:**

| API | Purpose |
|-----|---------|
| VirusTotal | URL scanning for malware and phishing detections |
| AbuseIPDB | IP address abuse confidence scoring |
| IPinfo | IP geolocation and organization lookup |
| IPQualityScore | IP fraud score and phishing flag |

**Risk Verdict Categories:**
- Phishing Site (High Risk)
- Slight Chance of Phishing (Medium Risk)
- Probably Safe (Low Risk)

## Repository Contents

```
Phishing_Detection_Tool_PPT.pptx
Documents/
├── Program Source Code/
│   ├── App.py                                  - Main application source code
│   └── config.ini                              - API key configuration
├── Data Analysis.pdf                           - Data analysis on captured results
├── Earned Value Sheet.xlsx                     - Project earned value tracking
├── Project_Plan.docx                           - Detailed project plan and timeline
├── Project Management Plan.pdf                 - Project management and communication plan
├── Risk_management_plan.pdf                    - Risk identification and mitigation plan
└── Links for the Github and Demo Video.docx    - Demo video and resource links
```

## How to Run

```
python App.py
```

Requires a `config.ini` file populated with valid API keys for VirusTotal, AbuseIPDB, IPinfo, and IPQualityScore.
