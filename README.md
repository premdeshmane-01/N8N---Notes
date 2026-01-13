# 8️⃣ n8n Notes & Workflows

![n8n](https://img.shields.io/badge/n8n-Workflow_Automation-orange?style=for-the-badge&logo=n8n)
![JavaScript](https://img.shields.io/badge/JavaScript-Code_Node-yellow?style=for-the-badge&logo=javascript)
![JSON](https://img.shields.io/badge/JSON-Data_Structure-lightgrey?style=for-the-badge&logo=json)

## 📖 About This Repository

Welcome to my personal knowledge base for **n8n** (nodemation). This repository serves as a collection of notes, code snippets, and exported workflow JSONs that I use to master workflow automation.

Whether you are looking for specific node configurations, JavaScript transformation snippets, or full automation logic, you will find it documented here.

## 🗂️ Repository Structure

The notes are organized by category to make navigation easy:

```text
├── 01-Concepts/          # Core concepts (Execution flow, Data structure)
├── 02-Nodes/             # Deep dives into specific nodes (HTTP Request, Switch, Merge)
├── 03-Code-Snippets/     # JavaScript/Python code for the 'Code' node
├── 04-Workflows/         # Full .json workflow exports ready to import
└── 05-Deployment/        # Notes on Docker, Self-hosting, and Environment Variables

```

🚀 Getting Started
Prerequisites
An active instance of n8n (Self-hosted or Cloud).

Basic understanding of JSON.

How to use these workflows
Navigate to the 04-Workflows folder.

Open the .json file of the workflow you want.

Copy the raw JSON content.

Open your n8n Editor canvas.

Press Ctrl + V (or Cmd + V on Mac) to paste the nodes directly into your canvas.

📝 Key Topics Covered
Data Transformation: Handling Arrays, Objects, and binary data.

The Code Node: Advanced logic using JavaScript/TypeScript.

API Integration: Authentication methods (Header Auth, OAuth2) and HTTP Requests.

Error Handling: Using Error Triggers and Try/Catch patterns in workflows.

Webhooks: Receiving data from external apps.

💡 specific Snippet Example
Example of a common transformation saved in this repo:

Flattening a nested JSON object:

```// Found in /03-Code-Snippets/flatten-json.js
return items.map(item => {
  return {
    json: {
      id: item.json.id,
      name: item.json.user.name,
      email: item.json.contact.email
    }
  }
});
```

🤝 Contributing
If you have a useful snippet or an optimization for a workflow:

Fork the repo.

Create a new branch (git checkout -b feature/amazing-snippet).

Commit your changes.

Push to the branch and open a Pull Request.

📄 License
This project is open-source and available under the MIT License.

Maintained by [Prem Deshmane]


### 3 Tips to make this repo stand out:

1.  **Use Screenshots:** In your `04-Workflows` folder, try to include a `.png` screenshot of what the workflow looks like in the canvas alongside the `.json` file.
2.  **Tagging:** If you use GitHub, add tags like `automation`, `low-code`, `n8n`, and `javascript` to the repo settings to make it discoverable.
3.  **The Code Node:** Since you have developer skills (React, JS, Python), focus heavily on the **"Code Node"** section. This is the hardest part for non-coders and the most valuable part for developers using n8n.
