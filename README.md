# Octra-Wallet-Generation
🪙 Wallet-Gen Setup Guide

To run this node, you will need to purchase a vps or run on local machine. All command will work on Windows Powershell.

# ✅ Prerequisites
Make sure your system has:

**. Git**

**. Node.js (v18 or later)**

**. npm (Node package manager)**

# Installation

```bash
sudo apt update
sudo apt install git nodejs npm -y
```

If your distro doesn't include a recent Node.js version, install it via NodeSource:

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
```
Install bun
```bash
curl -fsSL https://bun.sh/install | bash
```
Activate Bun in your current shell session
```bash
export BUN_INSTALL="$HOME/.bun"
export PATH="$BUN_INSTALL/bin:$PATH"
```
To make this permanent, add the lines below to your shell config
```bash
echo 'export BUN_INSTALL="$HOME/.bun"' >> ~/.bashrc
echo 'export PATH="$BUN_INSTALL/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

#verify Bun
bun --version
```
# Clone the Repository
```bash
git clone https://github.com/octra-labs/wallet-gen.git
cd wallet-gen
```
Install Repo
```bash
npm install
```
Build Repo
```bash
npm run build
```
It creates a binary named
```bash
wallet-generator
```

# Run the Wallet Generator
```bash
./wallet-generator -c 10 -o wallets.csv
```
If you get a permissions error, give the binary execute permission(Optional), if above command does not work
```bash
chmod +x wallet-generator
./wallet-generator -c 10 -o wallets.csv
```

# Open your browser to Access Localhost
```bash
http://localhost:8888
```


For VPS, you cannot acccess localhost from port above, you will need redirect the localhost.

Open a new window or VPS tab and run the code below.

**VPS Users can use Tunnel**

Install Tunnel
```bash
npm install -g localtunnel
```
Get Password(will be your vps IP)
```bash
curl https://loca.lt/mytunnelpassword
```
Get a new URL
```bash
lt --port 8888
```
Port is at 8888 by default, but if you changed the default port, replace 8888 with the new port.

Visit the given link, your password is your **VPS IP**

# Generate Wallet

After you login, 

Click on Generate wallet

Save your seedphrase, privatekey and public address

# Faucet
https://faucet.octra.network/
request once every 5 days

# Scan
https://octrascan.io/


**That's all for now, but any question, or problem you can reach me on X**

https://x.com/OamenJamiu






