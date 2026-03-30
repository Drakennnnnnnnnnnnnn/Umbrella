# 🛡️ Cisco Umbrella Recon Tool

<p align="center">
  <img src="https://giffiles.alphacoders.com/215/215910.gif" width="300" alt="Umbrella">
  <br>
  <strong>Tool to perform subdomain reconnaissance using Cisco APIs</strong>
</p>

---

## 🎯 Purpose of the Tool
This script leverages Cisco's global DNS traffic data, using its **API** to discover subdomains often missed by traditional brute-force methods or search engine indexing. By obtaining this data **passively**, it helps map a target's infrastructure and identify hidden or misconfigured assets.

---

## 🔑 Obtaining API Keys

To authenticate with the Cisco Umbrella APIs, follow these steps:

1. **Create Account:** Sign up at the [Umbrella Free Trial Portal](https://signup.umbrella.com/?utm_content=automated-free-trial).
2. **Navigate:** Log in to your dashboard and go to:
   * `Admin` ➡️ `API Keys`
3. **Generate:** Select the option to create a new key. Copy your **Access Key** and **Secret**.

---

## ⚙️ Environment Setup

We recommend storing your credentials as environment variables to keep them out of your script's source code.

```bash
# Add your credentials in "accesskey:secret" format
echo 'export UMBRELLA_TOKEN="your_access_key:your_secret"' >> ~/.bashrc

# Apply changes to your current terminal
source ~/.bashrc
```

## 🚀 How to use
Run the script directly from your terminal:

```bash
./umbrella_recon.sh targetdomain.com
```
