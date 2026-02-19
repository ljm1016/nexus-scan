NexusScan
The Bridge Between Threat Intel and Network Assets.

NexusScan is a modular, distributed cybersecurity pipeline designed to close the gap between what attackers are talking about (External Threat Intelligence) and what ports we have open (Internal Asset Monitoring).

Built as a collaborative project for the [Your Club Name] Cybersecurity Club.

The Architecture
NexusScan is split into four distinct "Blocks" so club members can contribute based on their interests:

Block A: The Ingestors (The "Hands") – Python scrapers pulling from CISA KEV, OSS-Security, and Mastodon.

Block B: The Scanner (The "Eyes") – Active and passive network discovery using RustScan and Nmap.

Block C: The ML Processor (The "Brain") – Named Entity Recognition (NER) to extract software versions from raw text.

Block D: The Dashboard (The "Voice") – Real-time threat visualization using Streamlit and Supabase.

Tech Stack
Database: Supabase (PostgreSQL + Realtime)

Languages: Python, SQL, (optional) Rust

Scanning: Nmap, RustScan, Shodan API

ML/NLP: spaCy, Hugging Face Transformers

Deployment: GitHub Actions (Automation)

How It Works
Scrapers find a new vulnerability (e.g., "Critical RCE in Apache 2.4.49").

Scanners identify a local asset (e.g., "192.168.1.15 is running Apache 2.4.49").

NexusScan joins these data points in Supabase.

The Dashboard triggers a high-priority alert for the Blue Team to patch.

Contributing
We are looking for members to join the following sub-teams:

Web Scrapers: Help us build robust Python scrapers.

Data Engineers: Manage the Supabase schema and API integrations.

ML Team: Train models to extract software versions from messy forum posts.

Security Analysts: Write remediation advice for the threats we find.
