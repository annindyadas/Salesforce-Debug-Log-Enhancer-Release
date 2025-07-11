# ⚡ Salesforce Debug Log Enhancer
“Stop guessing. Start debugging smarter.”

**Link to Download:**  
[Salesforce Debug Log Enhancer - Chrome Web Store](https://chromewebstore.google.com/detail/salesforce-debug-log-enha/bbmjihbifoabgfpbbembfecgdnhaibmn)

**Short Demo:**  
[Youtube Link](https://www.youtube.com/watch?v=wptRTgkUD78)

---

## 🧩 Problem Statement

Salesforce developers frequently struggle to identify the source of execution in lengthy and cryptic debug logs. The default Salesforce interface provides no direct visibility into which Apex class, method, trigger, flow, or Visualforce page initiated the log.

This lack of clarity leads to wasted time, slower debugging cycles, and frustration — especially when working across large codebases or in complex orgs.

---

## ✅ Solution: Debug Log Enhancer

Salesforce Debug Log Enhancer is a Chrome extension that automatically augments the standard Debug Logs page by identifying and displaying:

- 🔍 Type of execution (Apex, Trigger, Flow, Visualforce, etc.)
- 🧩 Class Name
- 🧠 Method Name

These are injected as new columns directly into the Salesforce Setup log table view — giving you instant context with zero clicks.

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| 🧠 Smart Parsing | Automatically fetches and analyzes each debug log detail page |
| 📊 Inline Column Injection | Adds Type, Class Name, and Method Name to the debug log table |
| ⚙️ Supports Multiple Execution Types | Apex Classes, Anonymous Blocks, Triggers, Flows, Visualforce, Packages |
| 🪶 Lightweight & Silent | Loads only on Salesforce Setup pages, adds no extra UI clutter |
| 🧪 Debug Mode Toggle | Optional logging for development and troubleshooting |
| 🔐 Secure | Requires minimal permissions, scoped only to Salesforce domains |

---

## 🔐 Privacy & Data Security

Your data is safe — always.

This extension:

- 🚫 Does NOT collect, transmit, or store any data from your Salesforce orgs
- 🚫 Does NOT log or track user interactions, credentials, or PII
- 📍 Only runs locally on your browser, enhancing the page interface client-side
- 🔐 Uses strict domain-scoped permissions (*.salesforce.com) to limit access

Your debug logs and org data never leave your device. This is a developer productivity tool — not a data service.

---

## 🌐 Compatibility

| Org Type | Supported |
|----------|-----------|
| Production Orgs | ✅ |
| Developer Editions | ✅ |
| Sandboxes | ✅ |
| Trailhead Playgrounds | ✅* |

Works on all Salesforce-hosted domains:

- *.lightning.force.com
- *.my.salesforce.com
- *.visualforce.com
- *.salesforce-setup.com

*Note: Trailhead Playgrounds using cross-domain iframes may restrict access due to browser security policies.

---

## 🧠 How It Works

1. On visiting the Debug Log listing page, the extension:
   - Detects and monitors the DOM for the debug log table
   - Extracts each log’s "View" link
   - Fetches the log detail page content
   - Parses and classifies execution source:
     - Apex Class & Method
     - Trigger Name & Event
     - Flow or Visualforce Page
     - Managed Package or Anonymous Block

2. Adds this data directly into new columns in the existing table — all within your browser

---

## 🛠 Tech Stack

- Manifest v3 (Chrome Extensions)
- Vanilla JavaScript
- Uses:
  - fetch API for log detail retrieval
  - MutationObserver for dynamic DOM changes
  - Regex-based parsing of log lines

---

## 🔐 Permissions Summary

| Permission | Purpose |
|------------|---------|
| host_permissions | Scoped to only Salesforce domains — no access to other sites |

---

## 👤 Author

**Annindya Das**  
Salesforce Developer & Platform Engineer

[Connect with me on LinkedIn](https://www.linkedin.com/in/annindya-das/)

---

## 📣 Feedback & Contributions

Want to add more log types like Scheduled Jobs, Batch Apex, or REST API calls?  
✨ Requests and ideas are welcome!

**GitHub Issues:**
[Submit Issues](https://github.com/annindyadas/Salesforce-Debug-Log-Enhancer-Release/issues)

**GitHub Releases:**
[View Releases](https://github.com/annindyadas/Salesforce-Debug-Log-Enhancer-Release/releases)

---

## ☕ Support My Work

💡 If you find this extension helpful, consider supporting my work by buying me a coffee:  
👉 [https://buymeacoffee.com/annindyadas](https://buymeacoffee.com/annindyadas)
