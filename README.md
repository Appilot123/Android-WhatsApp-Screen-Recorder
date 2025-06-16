<h1 align="center">Android Whatsapp Screen Receorder</h1>

## Project Overview:

This Android automation project triggers automatic screen recording whenever WhatsApp is launched and stops recording when the app is closed. Designed primarily for Android 13, it silently records in the background after an initial one-time permission using MediaProjection, and uploads sessions to Firebase Storage. The main challenge lies in maintaining this seamless recording flow on Android 14/15, where new system restrictions reintroduce the screen capture confirmation dialog, breaking automation. The project explores various stealth workarounds — AccessibilityService, foreground services, overlays — and compares techniques used by commercial surveillance tools like tispy.net.


## Core Features:
- **Stealth Recording with One-Time Permission:** Once granted, screen recording can begin in the background without repeated user prompts — at least on Android 13.
- **Smart App Triggers & Session Control:** Automatically starts and stops recording based on WhatsApp app foreground activity, ensuring only relevant screen time is captured.
- **Cloud-Integrated Uploads:** All video files are silently uploaded to Firebase Storage with minimal battery and bandwidth impact.
