<h1 align="center">Android Whatsapp Screen Receorder</h1>

## Project Overview:

This Android automation project triggers automatic screen recording whenever WhatsApp is launched and stops recording when the app is closed. Designed primarily for Android 13, it silently records in the background after an initial one-time permission using MediaProjection, and uploads sessions to Firebase Storage. The main challenge lies in maintaining this seamless recording flow on Android 14/15, where new system restrictions reintroduce the screen capture confirmation dialog, breaking automation. The project explores various stealth workarounds — AccessibilityService, foreground services, overlays — and compares techniques used by commercial surveillance tools like tispy.net.


## Core Features:
- **Stealth Recording with One-Time Permission:** Once granted, screen recording can begin in the background without repeated user prompts — at least on Android 13.
- **Smart App Triggers & Session Control:** Automatically starts and stops recording based on WhatsApp app foreground activity, ensuring only relevant screen time is captured.
- **Cloud-Integrated Uploads:** All video files are silently uploaded to Firebase Storage with minimal battery and bandwidth impact.

<div align="center">
  <img
    src="https://github.com/user-attachments/assets/d200549d-7613-446f-a43b-19a4117ca360"
    alt="select device"
    width="600px"
  />
</div>


<div align="center">
  <a href="https://appilot.app/">
    <img
      alt="Website"
      width="25px"
      src="https://github.com/user-attachments/assets/8e5f3af3-b098-4c1d-980d-df9aebc680d0"
    />
    <code>Appilot Website</code>
  </a>
  &nbsp;&nbsp;
  <a href="https://discord.gg/3CZ5muJdF2">
    <img
      alt="Join Our Server"
      width="30px"
      src="https://github.com/Zeeshanahmad4/RealEstateMate-WhatsApp-Group-Management-Bot/blob/main/discord-icon-svgrepo-com.svg"
    />
    <code>Join Our Server</code>
  </a>
  &nbsp;&nbsp;
  <a href="https://t.me/devpilot1">
    <img
      alt="Contact us"
      width="30px"
      src="https://edent.github.io/SuperTinyIcons/images/svg/telegram.svg"
    />
    <code>Contact Us</code>
  </a>
</div>

<div align="center">
<strong> Have a Custom Project in Mind please Contact?</strong>

<div align="center">
  <a href="mailto:support@appilot.app">
  <img
    alt="Email"
    width="30px"
    src="https://github.com/user-attachments/assets/91c8d428-32b7-4be0-91fa-2e42c902b5b8"
  />
  <code>support@appilot.app</code>
</a>
  &nbsp;&nbsp;
  <a href="https://cal.com/app-pilot-m8i8oo/30min">
  <img
    alt="Book a 30-minute Call"
    width="30px"
    src="https://github.com/user-attachments/assets/cd3e5c7b-3e4e-4bb3-b242-bcc20ee78f13"
  />
  <code>Book a 30-minute Call</code>
</a>
<span>

<div align="left">

## Features List:
| Feature                         | Description                                                                 |
| ------------------------------- | --------------------------------------------------------------------------- |
| Auto Trigger on WhatsApp Launch | Detects when WhatsApp is opened and starts recording automatically.         |
| MediaProjection Integration     | Uses Android's native screen recording API with one-time permission flow.   |
| Background Uploads to Firebase  | Seamless, low-latency upload of screen recordings to Firebase Storage.      |
| Android 13 Compatibility        | Works smoothly on Android 13 without repeat prompts after initial setup.    |
| Foreground Service Handling     | Ensures stable recording session even during app switches or interruptions. |
| AccessibilityService Hooks      | Experimental use of Accessibility to auto-confirm recording prompt.         |
| Overlay & Flag Tweaks           | Tested various permission flags to persist recording invisibly.             |


## Key Stats:
- **Automation Accuracy:** 98% on Android 13
- **Session Stability:** 4+ hours per recording without crash
- **Firebase Upload Success Rate:** 97%
- **Prompt Bypass Success (Android 14/15):** Currently 0% — under R&D


## Built Using:
- MediaProjection API
- Android AccessibilityService (Experimental)
- Foreground Services + Notification Channels
- Firebase Storage SDK
- Android 13–15 Testing (Non-Rooted)
