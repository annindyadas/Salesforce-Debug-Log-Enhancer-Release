⚡ Salesforce Debug Log Enhancer
“Stop guessing. Start debugging smarter.”

Link to Download: https://chromewebstore.google.com/detail/salesforce-debug-log-enha/bbmjihbifoabgfpbbembfecgdnhaibmn
_____________________________________________________________________________________
💡 If you find this extension helpful, consider supporting my work by buying me a coffee:
👉 https://buymeacoffee.com/annindyadas
________________________________________
🧩 Problem Statement
Salesforce developers frequently struggle to identify the source of execution in lengthy and cryptic debug logs. The default Salesforce interface provides no direct visibility into which Apex class, method, trigger, flow, or Visualforce page initiated the log.
This lack of clarity leads to wasted time, slower debugging cycles, and frustration — especially when working across large codebases or in complex orgs.
________________________________________
✅ Solution: Debug Log Enhancer
Salesforce Debug Log Enhancer is a Chrome extension that automatically augments the standard Debug Logs page by identifying and displaying:
•	🔍 Type of execution (Apex, Trigger, Flow, Visualforce, etc.)
•	🧩 Class Name
•	🧠 Method Name
These are injected as new columns directly into the Salesforce Setup log table view — giving you instant context with zero clicks.
________________________________________
✨ Features
Feature	Description
🧠 Smart Parsing - Automatically fetches and analyzes each debug log detail page
📊 Inline Column - Injection	Adds Type, Class Name, and Method Name to the debug log table
⚙️ Supports Multiple Execution Types	- Apex Classes, Anonymous Blocks, Triggers, Flows, Visualforce, Packages
🪶 Lightweight & Silent	- Loads only on Salesforce Setup pages, adds no extra UI clutter
🧪 Debug Mode Toggle	- Optional logging for development and troubleshooting
🔐 Secure	- Requires minimal permissions, scoped only to Salesforce domains
________________________________________
🔐 Privacy & Data Security
Your data is safe — always.
This extension:
•	🚫 Does NOT collect, transmit, or store any data from your Salesforce orgs
•	🚫 Does NOT log or track user interactions, credentials, or PII
•	📍 Only runs locally on your browser, enhancing the page interface client-side
•	🔐 Uses strict domain-scoped permissions (*.salesforce.com) to limit access
Your debug logs and org data never leave your device. This is a developer productivity tool — not a data service.
________________________________________
📦 Installation
1.	Download or clone this repo
2.	Open Chrome → go to chrome://extensions/
3.	Enable Developer Mode (top right)
4.	Click Load unpacked and select the extension folder
5.	Navigate to:
Setup → Debug Logs in your Salesforce org
✅ You’ll see new columns like Type, Class Name, and Method Name added
________________________________________
🌐 Compatibility
Org Type	Supported
Production Orgs	✅
Developer Editions	✅
Sandboxes	✅
Trailhead Playgrounds	✅*

Works on all Salesforce-hosted domains:
•	*.lightning.force.com
•	*.my.salesforce.com
•	*.visualforce.com
•	*.salesforce-setup.com
*Note: Trailhead Playgrounds using cross-domain iframes may restrict access due to browser security policies.
________________________________________
🧠 How It Works
1.	On visiting the Debug Log listing page, the extension:
o	Detects and monitors the DOM for the debug log table
o	Extracts each log’s "View" link
o	Fetches the log detail page content (<pre> section)
o	Parses and classifies execution source:
	Apex Class & Method
	Trigger Name & Event
	Flow or Visualforce Page
	Managed Package or Anonymous Block
2.	Adds this data directly into new columns in the existing table — all within your browser
________________________________________
🛠 Tech Stack
•	Manifest v3 (Chrome Extensions)
•	Vanilla JavaScript
•	Uses:
o	fetch API for log detail retrieval
o	MutationObserver for dynamic DOM changes
o	Regex-based parsing of log lines
________________________________________
🔐 Permissions Summary
Permission	Purpose
activeTab	Run only when Salesforce Setup tabs are open
scripting	Injects script into Salesforce pages
host_permissions	Scoped to only Salesforce domains — no access to other sites
________________________________________
👤 Author
Annindya Das
Salesforce Developer & Platform Engineer
Passionate about simplifying DevOps & debugging for the Salesforce ecosystem.
________________________________________
📣 Feedback & Contributions
Want to add more log types like Scheduled Jobs, Batch Apex, or REST API calls?
✨ Requests and ideas are welcome!

