# How to Run the Wallet Generator

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

If there is no access to port 8888, grant access with this command: ``` sudo ufw allow 8888 ```

**Open browser and go to:**
👉 http://serverip:8888 or http://localhost:8888 (if you use your pc)

# First task: Pre-Client

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
After running it you will see a user interface like this 

![image](https://github.com/user-attachments/assets/2d26c1b5-a31b-464b-bf50-1c8123dffdae)

**Now you can send token** 
If you wanna you can send me token ``` octDFCm6MYvDDz2k7Mn89Ftwap943xdMtqdE3NHcuQG6QyV ``` or check discord you'll see many address there.
You can check your TX here: https://octrascan.io/
