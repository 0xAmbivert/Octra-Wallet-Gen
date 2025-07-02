# Octra

# Wallet generation Guide

---

Copy and Paste these Commands on Codespace's Terminal One By One 

## 🔹 Step 1:

```bash
curl -fsSL https://bun.sh/install | bash
source ~/.bashrc
bun --version
````

---

## 🔹 Step 2:

```bash
bun install
```

---

## 🔹 Step 3:

```bash
bun run build
```

---

## 🔹 Step 4:

```bash
bun start
```

> click the **“PORTS”** tab open link under forwarded address in browser

---

**Wallet Generated, Back up private key**

Go to https://faucet.octra.network/

Paste Wallet address & claim faucet

Join Discord - https://discord.gg/WUghrsuywU

---



Octra Testnet Client Installation Guide for Windows 10
Copy and Paste these Commands in Command Prompt One By One

🔹 Step 1: Install Python
Install Python 3.8+ to run the Octra client:

cmd

Collapse

Wrap

Copy
:: Download Python from python.org (e.g., Python 3.11)
:: Run installer, check "Add Python to PATH", click Install Now
python --version
Should show Python 3.11.4 or similar

🔹 Step 2: Install Git
Install Git to clone the client repository:

cmd

Collapse

Wrap

Copy
:: Download Git from git-scm.com
:: Run installer with defaults, ensure "Git Bash Here" is enabled
git --version
Should show git version 2.41.0.windows.1

🔹 Step 3: Clone Client Repository
Clone the Octra client and set up the environment:

cmd

Collapse

Wrap

Copy
mkdir octra-testnet
cd octra-testnet
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
🔹 Step 4: Configure Wallet
Set up your wallet for the client:

cmd

Collapse

Wrap

Copy
copy wallet.json.example wallet.json
Open C:\Users\<YourUsername>\octra-testnet\octra_pre_client\wallet.json in Notepad
Add your private key and address (from wallet generation):
json

Collapse

Wrap

Copy
{
  "priv": "your-private-key-here",
  "addr": "your-oct-wallet-address-here",
  "rpc": "https://octra.network"
}
Save and close

🔹 Step 5: Run Client and Send Transactions
Run the client and send test transactions:

cmd

Collapse

Wrap

Copy
python cli.py
In the terminal UI, select “Send Tokens”
Enter address: oct6oJMJ8etECjhiEUrJVEfUfVDwQHuPLxgj45aPkB2wZXp
Send 1 OCT, confirm
Check transaction in the testnet explorer (find via @octra’s X)
Repeat with 2–3 addresses from Octra’s Discord

🔹 Step 6: Join Community
Join Octra’s Discord and Telegram (find invites on @octra’s X, June 26, 2025)
Share feedback, report bugs (e.g., “Client crashed, fixed by restarting”)
Follow @octra on X for new tasks
