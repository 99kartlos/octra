# Octra Testnet Tasks

![image](https://github.com/user-attachments/assets/08751c61-b0fb-4590-a090-ff37dac685b1)

**Twitter:** https://x.com/octra

**Discord:** https://discord.gg/octra

------

# Let's Generate Wallet

**Clone the repository and go into the folder:**

```sh
git clone https://github.com/octra-labs/wallet-gen.git
cd wallet-gen
```

**Start the wallet generator:**

On Linux/macOS:
```sh
chmod +x ./start.sh
./start.sh
```
On Windows:

```sh
start.bat
```

If there is no access to port 8888, get access with this command: ``` sudo ufw allow 8888 ```

**Open browser and go to:**

👉 http://serverip:8888 or http://localhost:8888 (if you not use VPS)

**Now you can get Faucet**

Visit Faucet page and Enter your address.. : https://faucet.octra.network/
Enter your address..

![image](https://github.com/user-attachments/assets/b847625d-6da5-4c7d-8ed6-ce1149324f04)

------

# First task:

**First let's setup python libraires**

```sh
sudo apt install python3 python3-pip python3-venv python3-dev -y
```

**Run the following commands one by one:**

```sh
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
python3 -m venv venv
source venv/bin/activate     # On Windows, use: venv\Scripts\activate
pip install -r requirements.txt
cp wallet.json.example wallet.json
```

**Open the file wallet.json and replace the placeholders with your actual wallet info:**

```sh
nano wallet.json
```
```sh
{
  "priv": "your-private-key-here", (B64 format)
  "addr": "your-octra-address-here", (oct...)
  "rpc": "https://octra.network"
}
```
**Run the project:**

On Linux/macOS:
```sh
./run.sh
```
On windows
```sh
run.bat
```   

After running it you will see a user interface like this 

![image](https://github.com/user-attachments/assets/2d26c1b5-a31b-464b-bf50-1c8123dffdae)

**Now you can send token** 

If you wanna you can send me token ``` octDFCm6MYvDDz2k7Mn89Ftwap943xdMtqdE3NHcuQG6QyV ``` or check discord you'll see many address there.
You can check your TX here: https://octrascan.io/
