# INVA Career Mode – PIREP Logger

The **INVA Career Mode – PIREP Logger** is a browser-based application designed to streamline Pilot Report (PIREP) submissions for Indian Virtual (INVA) pilots.  
It provides a structured, user-friendly interface for recording flight details, generating standardized receipts, and securely logging each record into a centralized database.

This repository contains only the front-end source code and supporting documentation.  
All sensitive information, backend configurations, tokens, and data endpoints are intentionally excluded to maintain security and integrity.

## Project Overview

This application enables INVA pilots to:
- Enter essential flight data such as flight number, route, aircraft type, duration, passengers, and cargo.  
- Generate a professionally formatted receipt with calculated totals and summary details.  
- Access a QR code for quick link sharing.  
- Automatically log all submitted data into a protected Google Sheet through a secure Apps Script endpoint.

All calculations and data handling are processed client-side, with results transmitted securely for logging and review.

## Key Features
- Clean and responsive web interface  
- Secure data submission with token verification  
- Auto-generated, printable receipts  
- QR-based share link for quick access  
- Structured data storage in Google Sheets  
- Designed exclusively for INVA Career Mode operations

## Repository Structure
INVA-PIREP-Logger/
├── index.html # Main front-end interface
├── assets/ # Logos and fonts
│ └── INVA Brand Logo.png
├── README.md # Project overview
└── LICENSE.txt # Credits and terms of use

pgsql
Copy code

## Deployment Overview
1. Frontend Hosting: deploy `index.html` and `assets/` using GitHub Pages or any static host.  
2. Backend Setup: deploy the Google Apps Script as a Web App with access set to “Anyone with the link”.  
3. Configuration: update the front-end constants (endpoint URL, token) in your private deployment.  
4. Validation: submit a test entry and confirm it appears in the designated Google Sheet.

> This repository does not contain backend credentials, tokens, or live sheet identifiers.

## Technology Stack
| Component  | Technology                  |
|------------|------------------------------|
| Frontend   | HTML, CSS, JavaScript        |
| Backend    | Google Apps Script (Web App) |
| Storage    | Google Sheets                |
| Deployment | GitHub Pages                 |

## Intended Use
This tool is designed for simulation and administrative purposes within the **Indian Virtual (INVA)** Career Mode.  
It has no real-world financial or operational validity and should not be used outside of its designated environment.

## License and Credits
This project is proprietary and developed exclusively for INVA.  
See [LICENSE.txt](LICENSE.txt) for full terms, credits, and usage restrictions.

© 2025 Jonathan Reeves. All Rights Reserved.
