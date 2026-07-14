# Social-Media-Footprint-Analysis
An OSINT (Open-Source Intelligence) assessment of the publicly available social media footprint of an authorized personal account, performed on Kali Linux using Sherlock and Maigret. The goal was to identify what information is discoverable from a single username, evaluate the privacy/security implications, and produce recommendations to reduce unnecessary exposure.

## Objectives
- Identify publicly accessible social media profiles tied to a target username
- Determine what information can be collected using OSINT tooling
- Demonstrate ethical OSINT investigation techniques
- Produce a professional security assessment report

## Target
Personal accounts owned by the researcher (self-assessment only — no third-party or unauthorized targets).

### Install Sherlock (Kali built-in package)
sudo apt update && sudo apt install sherlock -y

### Install Maigret's build prerequisites
sudo apt update && sudo apt install -y libcairo2-dev pkg-config python3-dev build-essential pipx

### Set up pipx and install Maigret
pipx ensurepath
pipx install maigret

### Run a full search and generate an HTML/PDF dossier
maigret {name} --html --pdf
