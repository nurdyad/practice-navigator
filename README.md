BetterLetter Practice Navigator
Overview
The BetterLetter Practice Navigator is a powerful Chrome extension designed to streamline navigation within the BetterLetter AI admin panel. It provides quick access to practice settings, mailroom sections (Preparing, Rejected), and user management by simply entering a practice name or ODS code. It also includes features for searching practices by CDB and viewing real-time practice status (EHR Type, Collection Quota, Collected Today, Service Level).

This extension is built to enhance productivity for BetterLetter AI administrators and support staff by minimizing manual navigation and data lookup.

Features
Quick Practice Navigation: Open specific practice settings tabs (Basic, Service, Workflows, EHR Settings) directly.

Mailroom Access: Jump directly to "Preparing" or "Rejected" mailroom queues for a specific practice.

User Management: Access the user list for a selected practice.

Intelligent Search: Find practices by name (with auto-suggestions) or ODS code.

CDB Search: Efficiently locate practices by their Practice CDB.

Real-time Status: View essential practice details like EHR Type, Collection Quota, Collected Today, and Service Level directly in the popup.

Cached Data: Utilises persistent caching to speed up lookups and reduce repetitive scraping.

Background Operations: Performs data scraping in background tabs to minimize disruption.

Repository Structure
BetterLetter-Practice-Navigator/
├── icons/
│   ├── icon-16.png
│   ├── icon-48.png
│   └── icon-128.png
├── floating_window.html
├── background.js
├── manifest.json
└── popup.js


manifest.json: The manifest file defining the Chrome extension's properties, permissions, and script references.

background.js: The service worker script, handling background logic, data scraping, caching, and inter-script communication.

popup.js: The script for the extension's popup UI (floating_window.html), managing user interactions, suggestions, and displaying information.

floating_window.html: The HTML structure for the extension's user interface (the popup window).

icons/: Directory containing various sizes of the extension icon.

Installation Guide (for Chrome)
Follow these steps to install the BetterLetter Practice Navigator extension in your Chrome browser:

1. Download the Extension Files
Clone this Git repository or download the source code as a ZIP file and extract it to a local folder on your computer.

git clone <repository-url>
cd BetterLetter-Practice-Navigator


(Replace <repository-url> with the actual URL of your Git repository.)

2. Open Chrome Extensions Page
Open your Google Chrome browser.

Type chrome://extensions into the address bar and press Enter.

3. Enable Developer Mode
On the Chrome Extensions page, locate the "Developer mode" toggle switch, usually found in the top right corner. Turn it ON.

4. Load the Extension
After enabling Developer mode, three new buttons will appear: "Load unpacked", "Pack extension", and "Update".

Click the "Load unpacked" button.

A file dialog will open. Navigate to the folder where you extracted or cloned the BetterLetter-Practice-Navigator repository (the folder containing manifest.json, background.js, popup.js, etc.).

Select this entire folder and click "Select Folder" (or "Open" on some systems).

5. Verify Installation
The "BetterLetter Practice Navigator" extension should now appear in your list of installed extensions.

You will see its icon in your Chrome toolbar (it might be hidden in the puzzle piece icon, if you have many extensions).

6. Pin the Extension (Optional, Recommended)
For easy access, you can "pin" the extension to your Chrome toolbar:

Click the puzzle piece icon (Extensions icon) in your Chrome toolbar.

Find "BetterLetter Practice Navigator" in the list.

Click the pin icon next to it. The extension icon will now be permanently visible in your toolbar.

7. Usage
Click the extension icon in your toolbar to open the floating navigation window.

Start typing a practice name or ODS code, or use the CDB search field.

Select a practice from suggestions or search results to enable contextual buttons.

Click the desired button (Open Settings, Users, Preparing, Rejected, Status, etc.) to navigate or view information.
