# N8N-Workflows 🚀  

<p align="center">
  <a href="https://github.com/selvaganesh19/N8N-Workflows/stargazers">
    <img src="https://img.shields.io/github/stars/<username>/N8N-Workflows?style=social" alt="Stars">
  </a>
  <a href="https://github.com/selvaganesh19/N8N-Workflows/network/members">
    <img src="https://img.shields.io/github/forks/<username>/N8N-Workflows?style=social" alt="Forks">
  </a>
  <a href="https://github.com/selvaganesh19//N8N-Workflows/issues">
    <img src="https://img.shields.io/github/issues/<username>/N8N-Workflows" alt="Issues">
  </a>
  <a href="https://github.com/selvaganesh19//N8N-Workflows/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License">
  </a>
  <img src="https://img.shields.io/badge/N8N-v1.0-blue" alt="N8N Version">
</p>

> **A curated collection of ready‑to‑use N8N workflows that streamline everyday automation tasks.**  
> From simple form‑driven responses to complex multi‑step pipelines, these workflows give you a head‑start in automating your processes.  
> The repository also contains a **Railway ticket pre‑booking** workflow that captures traveler data via a web form, validates it, and forwards it to your ticketing system.

If you find this repo helpful, please give it a star ⭐ — it helps other developers discover useful automations!

---

## ✨ Features  

- 🚀 **Ready‑to‑import N8N JSON files** – Drop them into your N8N instance and start running instantly.  
- 📦 **Diverse use cases** – Forms, webhooks, data enrichment, notifications, integrations with popular SaaS tools.  
- 🎫 **Railway pre‑booking workflow** – Demonstrates a full‑stack ticket reservation flow: form → validation → ticketing API.  
- 🧩 **Modular design** – Each workflow is self‑contained, making it easy to customize or extend.  
- 📚 **Comprehensive documentation** – Every workflow includes a short guide inside its JSON metadata.  
- 🌱 **Community‑driven** – Open for contributions, issues, and suggestions.

---

## 🛠️ Installation  

> **Prerequisites**  
> - An up‑to‑date N8N instance (v0.180+).  
> - Git (optional, for cloning).  

### 1️⃣ Clone the repository  

```bash
git clone https://github.com/selvaganesh19/N8N-Workflows.git
cd N8N-Workflows
```

> Replace `<username>` with your GitHub username (or the owner of this repo).  

### 2️⃣ Import a workflow  

1. Open your N8N UI (`http://localhost:5678` if running locally).  
2. Click **“+ New workflow”** → **“Import from file”**.  
3. Select the JSON file you want (e.g., `railway-pre-booking-trigger.json`).  
4. Click **“Import”** – the workflow appears in your canvas, ready to be configured.

> **Tip:** After importing, double‑check node credentials (API keys, webhook URLs, etc.) before activating the workflow.

### 3️⃣ (Optional) Install via Git Submodule  

If you keep N8N workflows in a separate folder, you can add this repo as a submodule:

```bash
git submodule add https://github.com/selvaganesh19/N8N-Workflows.git workflows
```

---

## 📖 Usage  

### Example: Railway ticket pre‑booking  

1. **Activate the workflow** after importing `railway-pre-booking-trigger.json`.  
2. **Configure the form node** (if you changed the form title/description).  
3. Set **webhook URLs** for your ticketing service (e.g., a REST endpoint).  
4. **Test the workflow**:  
   - Click **“Execute workflow”**.  
   - Submit the form; you should see the payload logged in the **Console** node.  
   - Verify that the data reaches your ticketing API (check the response in the **HTTP Request** node).  

> **Customize** the validation rules inside the **Function** node to match your business logic (e.g., date ranges, seat preferences).

### General tips  

- **Use environment variables** for secrets (N8N supports them via `{{ $env.VARIABLE }}`).  
- **Leverage the built‑in error handling** (set “Continue on fail” or add a **Stop and Error** node).  
- **Duplicate workflows** to experiment without affecting production ones.

---

## 🤝 Contributing  

We welcome contributions! 🎉  

### How to contribute  

1. **Fork** the repo on GitHub.  
2. **Create a feature branch**:  
   ```bash
   git checkout -b feature/awesome-workflow
   ```  
3. **Add your workflow** in a sub‑folder (e.g., `marketing/lead‑scoring.json`).  
4. **Update the README** if you add a new workflow (add a short description under ✨ Features).  
5. **Commit** your changes:  
   ```bash
   git commit -m "Add lead‑scoring workflow"
   ```  
6. **Push** and open a **Pull Request**.  

### Guidelines  

- ⭐ Keep each workflow **self‑contained** (no hidden dependencies).  
- 📝 Include **metadata** (`name`, `description`, `nodes` explanations).  
- 🧪 Test the workflow in a fresh N8N instance before submitting.  
- 🗝️ Never commit real API keys or credentials. Use environment variables.  

For bugs or feature requests, open an **Issue** and fill out the template.

---

## 📜 License  

This project is licensed under the **MIT License** – see the [LICENSE](https://github.com/selvaganesh19/N8N-Workflows/blob/main/LICENSE) file for details.

---

### 🌟 Show your support

If this repository saves you time, consider:

- ⭐ **Starring** it so others can discover it.  
- 🔄 **Sharing** a workflow with your team or on social media.  
- 🤝 **Contributing** your own automations to grow the collection.

> *Happy automating!* 🚀  

---  

**Maintainer:**  
- 👤 `Selvaganesh19` – feel free to reach out via GitHub Issues.  

---  

<!-- Replace all occurrences of `<username>` and `<Your Name>` with your actual details before publishing. -->

## License
This project is licensed under the **MIT** License.

---
🔗 GitHub Repo: https://github.com/selvaganesh19/N8N-Workflows