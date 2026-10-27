# RichTools Student & Developer Marketplace 🛒

Official dynamic marketplace catalog and extension registry for **RichTools - Richfield Student Hub**.

This repository hosts the manifest schemas, tool definitions, community plugins, and verified student developer extensions consumed dynamically by the RichTools desktop client.

---

## 🌟 Catalog Structure

- **[`catalog.json`](./catalog.json)**: The root catalog consumed live by RichTools clients. Includes verified developer tools, enterprise suites, and student plugins.
- **[`schema.json`](./schema.json)**: Strict JSON schema defining the metadata standards for all tools, wings, and subactions.
- **`extensions/`**: Source manifests and bundles for community extensions and campus tools.

---

## 🛠️ Included Categories

1. **Developer Tools**: Visual Studio Code, Git for Windows, Node.js LTS, Docker Desktop, Postman.
2. **Productivity & Office**: Microsoft 365 (Word, Excel, PowerPoint, Outlook), OneNote.
3. **Data Science & AI**: Anaconda Distribution, JupyterLab, Conda environments.
4. **Richfield Extensions**: SMOWL Proctoring Companion, Richfield Moodle Productivity Companion, Richfield GPA & Assessment Tracker.

---

## 🚀 Adding / Updating a Tool

Community contributors and campus developers can submit new tools or extension manifests via Pull Request:

1. Fork this repository.
2. Add your tool entry to `catalog.json` adhering to `schema.json`.
3. Provide a valid `wingetPackageId` or direct `downloadUrl`.
4. Ensure all `subActions` reference verified executables or shell commands.
5. Submit a PR. Automated tests validate `catalog.json` syntax and schema conformance.

---

## 🔗 Live Raw Endpoint

RichTools connects to the raw GitHub endpoint:
```text
https://raw.githubusercontent.com/modded-soldier-9/RichTools-Marketplace/main/catalog.json
```
If a student workstation is offline or firewalled, RichTools automatically falls back to its built-in local cache.

---

© 2026 Richfield Graduate Institute of Technology & RichTools Contributors.
