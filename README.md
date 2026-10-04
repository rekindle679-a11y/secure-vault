# SecureVault - Professional Cloud Security Platform

SecureVault is an enterprise-grade document security and encrypted storage platform built with React, Tailwind CSS, and Firebase (Authentication, Cloud Firestore, and Cloud Storage).

## Features

- **Multi-Factor / Clearance Authentication**:
  - Direct Google OAuth Popup (`firebase.auth.GoogleAuthProvider`)
  - Clearance ID / Email & Password authentication with strict Firebase verification
- **Private Sector Classification**:
  - Categorize documents under customizable sectors (Identity, Education, Finance, Health, Travel, Legal, Employment, etc.)
  - Create and delete custom private sectors with automatic cascade management
- **Real-Time Encrypted Storage**:
  - Live persistence with Firebase Firestore subcollections (`users/{uid}/vault_documents/{docId}`)
  - IndexedDB offline caching replica for lightning-fast responsiveness
- **Live Document Viewer**:
  - In-app preview for images and PDF documents
  - Document renaming, favoriting, and secure local extraction/download
- **Recycle Bin & Safe Purge**:
  - Soft-delete staging area with one-click restore and permanent cloud purge

## Tech Stack

- **Frontend**: React 18, Tailwind CSS, FontAwesome 6.5.1
- **Backend**: Firebase Authentication, Cloud Firestore, Cloud Storage, Firebase Analytics
- **Local Cache**: IndexedDB Engine

## Getting Started

1. Serve `index.html` via any HTTP web server (e.g. Python):
   ```bash
   python3 -m http.server 8080
   ```
2. Open [http://localhost:8080](http://localhost:8080) in your web browser.
3. Authenticate with Google or create a Clearance ID to access your secure vault.
