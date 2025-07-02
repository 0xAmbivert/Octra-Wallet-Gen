# Octra

# Wallet Generation Guide

---

Copy and Paste these Commands on Command Prompt or Codespace's Terminal One By One

## 🔹 Step 1:
Install Bun to generate the wallet:
```cmd
curl -fsSL https://bun.sh/install | bash
source ~/.bashrc
bun --versionShould show Bun version (e.g., 1.0.0)🔹 Step 2:Set up the project:bun install🔹 Step 3:Build the wallet:bun run build🔹 Step 4:Start the wallet generator:bun startClick the “PORTS” tab, open the link under forwarded address in browserWallet Generated, Back Up Private KeyCopy your wallet address (starts with "oct"), private key, and mnemonic phraseSave in a secure file (e.g., Notepad as octra_wallet.txt on a USB drive)Never share your private key or mnemonicClaim FaucetGo to the Octra faucet (find via @octra’s X, June 26, 2025)Paste your wallet address, click “Request Tokens”Wait 2-5 minutes, check balance in testnet explorerJoin CommunityJoin Octra’s Discord (find invite on @octra’s X, June 26, 2025)Follow @octra on X for updatesClient Installation Guide for Windows 10Copy and Paste these Commands in Command Prompt One By One🔹 Step 1: Install PythonInstall Python 3.8+ to run the Octra client::: Download Python from python.org (e.g., Python 3.11)
:: Run installer, check "Add Python to PATH", click Install Now
python --versionShould show Python 3.11.4 or similar🔹 Step 2: Install GitInstall Git to clone the client repository::: Download Git from git-scm.com
:: Run installer with defaults, ensure "Git Bash Here" is enabled
git --versionShould show git version 2.41.0.windows.1🔹 Step 3: Clone Client RepositoryClone the Octra client and set up the environment:mkdir octra-testnet
cd octra-testnet
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt🔹 Step 4: Configure WalletSet up your wallet for the client:copy wallet.json.example wallet.jsonOpen C:\Users\<YourUsername>\octra-testnet\octra_pre_client\wallet.json in NotepadAdd your private key and address (from wallet generation):{
  "priv": "your-private-key-here",
  "addr": "your-oct-wallet-address-here",
  "rpc": "https://octra.network"
}Save and close🔹 Step 5: Run Client and Send TransactionsRun the client and send test transactions:python cli.pyIn the terminal UI, select “Send Tokens” Enter address: oct6oJMJ8etECjhiEUrJVEfUfVDwQHuPLxgj45aPkB2wZXp Send 1 OCT, confirm Check transaction in the testnet explorer (find via @octra’s X) Repeat with 2–3 addresses from Octra’s Discord🔹 Step 6: Join CommunityJoin Octra’s Discord and Telegram (find invites on @octra’s X, June 26, 2025)Share feedback, report bugs (e.g., “Client crashed, fixed by restarting”)Follow @octra on X for new tasks