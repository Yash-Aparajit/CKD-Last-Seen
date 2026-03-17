# CKD Material Last Seen System

A lightweight industrial web application to track last known physical movement of CKD material using QR scan.

## Purpose

Prevent false shortage escalation by providing real-time last seen information of parts inside plant.

This system is NOT an ERP replacement.

It provides:

- Material visibility
- Picker movement signal
- Packing delay detection
- Shortage investigation data

## Features

- QR scan based material logging
- Last seen search by Part ID
- Multi-location tracking (Store / Table / Reput Away)
- Excel report export with filters
- Mobile friendly UI
- Firebase serverless backend

## Tech Stack

- Firebase Firestore
- Firebase Hosting
- HTML5 QR Scanner
- SheetJS Excel Export
- Vanilla JS

## Deployment

1. Install Firebase CLI
2. `firebase init`
3. Place index.html inside public folder
4. `firebase deploy`

## Industrial Workflow

1. Picker scans when material leaves store
2. Packing uses material
3. If shortage suspected → search in app
4. Management exports Excel for analysis

## Limitations

- Requires internet connectivity
- No authentication (pilot phase)
- No offline buffering (future version)

## Future Upgrades

- Offline sync
- Shortage probability model
- Picker authentication
- Dashboard analytics
- Lot-level tracking
