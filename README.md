# Delivery-Reminder-for-iOS
This is an advanced Apple Shortcut that uses AI to intelligently read delivery and courier text messages, extract the delivery location and pickup code, and automatically create a detailed reminder in your Apple Reminders app.
## The Problem
### Tired of receiving a text like this?

"【xx驿站】您的快递已到xx驿站,请凭xx-xx-xxxx及时取件。"

Manually copying the location and code, opening Reminders, creating a new item, and setting a time is tedious. This shortcut automates the entire process in one or two clicks.

## Key Features
**Intelligent AI Parsing:** Uses AI API to understand unstructured text and find the key information.

**Extracts Critical Data:** Grabs both the location and the pickup code, creating a detailed reminder title like: 拿快递：x驿站 (取件码: xx-xx-xxx).

**Automatic Time:** Automatically sets the reminder for 6:00 PM on the same day.

**Robust AI Handling:** Includes advanced RegEx matching to "clean" the AI's JSON output, making it reliable even when the AI returns messy Markdown (e.g., ```json...```).

Cross-Platform Workarounds: Provides two different trigger methods to work perfectly on both iOS and macOS.

## IMPORTANT: Setup Instructions
This shortcut will not work until you add your own API key.

**Get a LLM API Key:** Go to Google AI Studio/OpenAI/DeepSeek, sign in, and create a new, free API key.

**Download the Shortcut:** Install this shortcut on your iPhone and/or Mac.

**Paste Your Key:**

- Open the Shortcuts app and edit this shortcut.

- Find the Text action near the very top.

- Replace the placeholder text **PASTE_YOUR_OWN_API_KEY_HERE** with your actual API key.

## How to Use
This shortcut is designed to be run in two different ways, depending on your device.

1. On iOS (The "Share Sheet" Method)

This is the fastest and most elegant method.

In the Messages (信息) app, long-press on the message bubble (do not select the text inside).

A menu will appear. Tap Share... (共享...).

In the Share Sheet that pops up, scroll down and tap the name of this shortcut.

Done! The shortcut will run and create the reminder.

2. On macOS (The "Clipboard + Menu Bar" Method)

This method is a required workaround for a macOS bug where the Share Sheet is not allowed to make network calls (which blocks the AI).

First-Time Setup: In the Shortcuts app on your Mac, edit this shortcut, click the (i) icon, and check Pin in Menu Bar (在菜单栏中置顶).
