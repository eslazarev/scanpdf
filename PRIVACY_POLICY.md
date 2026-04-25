# Privacy Policy for ScanPDF

**Last Updated:** April 25, 2026

## Introduction

ScanPDF ("we," "our," or "the app") is an on-device document scanning application that converts photos of paper documents into multi-page PDF files. This Privacy Policy explains how ScanPDF handles information.

## Information We Collect

### Document Images
- **Page captures:** When you actively start a scan, ScanPDF (via Google ML Kit Document Scanner) captures photographs of pages through your device's camera.
- **Generated PDFs:** Captured pages are combined into a multi-page PDF file.

### What we do NOT collect
- No personal information
- No biometric data
- No location data
- No contacts
- No usage analytics
- No advertising identifiers
- No account or login data

## How We Use Your Information

ScanPDF uses captured documents solely for:
- Producing a PDF file from your scan
- Displaying a preview of the resulting PDF
- Sharing the PDF when you explicitly tap "Share"

## Data Storage

### Local Storage Only
**All scans and PDFs are stored exclusively on your device.** ScanPDF operates entirely on-device and does not:
- Transmit your scans to any developer-operated server
- Use cloud storage
- Share data with third parties (unless you explicitly choose to share via Android's share sheet)
- Require an account or login

Files are stored in:
- The app's private `filesDir/scans/` directory (final multi-page PDFs)
- The app's private `filesDir/staging/` directory (temporary capture files)

### Data Security
- All files live in the app's private storage area, inaccessible to other applications
- The app declares `android:allowBackup="false"` so PDFs are not included in Android Auto Backup or `adb backup`
- The app declares no network permissions for its own use

### Third-Party Services
- **Google ML Kit Document Scanner:** Provides the camera UI, edge detection, perspective correction, filters, and PDF assembly. Runs entirely on-device. The first time you scan, Google Play services may download the scanner module from Google Play. After that no internet is required.
- **No other third-party SDKs** - no analytics, no crash reporting, no ads, no tracking.

### No Remote Access
The developer has no ability to access, view, modify, or delete any data stored by this app. ScanPDF:
- Does not connect to any developer-operated server
- Has no backend infrastructure
- Stores all data exclusively on your local device

## Sharing

When you tap "Share PDF" in the app, ScanPDF passes the PDF to Android's system share sheet. From there you choose the destination (Gmail, Drive, WhatsApp, and so on). The receiving app handles the file according to its own privacy practices. ScanPDF cannot see or control what happens after sharing.

## Permissions

- **Camera:** Requested by Google ML Kit's scanner Activity at the moment you start a scan. ScanPDF does not access the camera outside of this flow.
- **Storage:** No external-storage permissions are requested. All files stay in app-private storage.
- **Internet:** Not declared in the app's Manifest. Used only by Google Play services to fetch the scanner module on first run, governed by Google Play's own permissions.

## Data Retention

- PDFs you create remain on your device until you delete them or uninstall the app.
- Uninstalling ScanPDF removes all stored data.

## Children's Privacy

ScanPDF is suitable for general audiences. The app does not knowingly collect any information from any users, including children under 13.

## Your Rights

Since all data is stored locally on your device and the developer has no access to it, requests regarding your personal data are handled directly by you:
- View what is stored: open the Preview screen, or browse Android's per-app storage info
- Delete: uninstall the app

## Changes to This Privacy Policy

We may update this Privacy Policy from time to time. Any changes will be reflected in the "Last Updated" date at the top of this document. Continued use of the app after changes constitutes acceptance of the updated policy.

## Compliance

This app is designed to support compliance with:
- General Data Protection Regulation (GDPR)
- California Consumer Privacy Act (CCPA)
- Other applicable data protection laws

Because no data leaves your device, most data subject rights are already satisfied at the design level.

## Contact

**Developer:** Evgenii Lazarev
**GitHub:** https://github.com/eslazarev/pdf-pro
**Email:** eslazarev@gmail.com

---

## Summary

| Data Type | Collected | Stored Locally | Sent to Servers | Retention |
|-----------|-----------|----------------|-----------------|-----------|
| Page photos | Yes (when you scan) | Yes | No | Until uninstall |
| Generated PDFs | Yes | Yes | No | Until uninstall |
| Personal info | No | - | - | - |
| Analytics | No | - | - | - |

**Key Points:**
- All data stays on your device
- ScanPDF never connects to a developer-operated server
- The developer cannot remotely access or delete your data
