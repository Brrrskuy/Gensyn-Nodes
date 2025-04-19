# <h2 align=center>Gensyn Nodes Guides </h2>
- **Buy VPS in** : [t.me/skuycloud](t.me/skuycloud)
- **Trakteer buy Kopi** : https://trakteer.id/brrrskuy/tip `<---`

| **Requirement**                                    |
|----------------------------------------------------|                      
|  **16GB RAM**                                      |
|  **CUDA Devices  RTX 3090, RTX 4090, A100, H100**  |
|  **Python Version	>= 3.10**                        |

**1. First time `If your VPS 8GB/4c` and you want RUN it :D + VPS fresh you can `install this as not be Killed` https://github.com/Brrrskuy/Overcommit-Extreme-RAM.CPU**


**2. Install Version Nodejs v20.0 `if Installed skip this`**
```
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
```
```
sudo apt install -y nodejs
```
`Check your version nodejs`
```
node -v
```
**3. Install Dependencies**
```
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl screen git yarn && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn
```
**4. Clone Repository**
```
git clone https://github.com/gensyn-ai/rl-swarm.git && cd rl-swarm
```
**5. Create Screen**
```
screen -S gensyn
```
**6. Run Script RL Swarm**
```
python3 -m venv .venv && source .venv/bin/activate && ./run_rl_swarm.sh
```
`Would you like to connect to the Testnet? [Y/n] Y`

**`If Output like this`**

![image](https://github.com/user-attachments/assets/8287cc36-5425-4eb5-b17a-1d1115119c1b)

**7. Use Ngrok for OTP/URL**

![image](https://github.com/user-attachments/assets/a9c09501-65cb-4b12-9e65-8eb9bfc8bf00)

`Open same VPS IP and Paste code below on new tab your IP VPS`

`Don't close proviuse tab`
```
wget https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-v3-stable-linux-amd64.tgz && tar -xvzf ngrok-v3-stable-linux-amd64.tgz && sudo mv ngrok /usr/local/bin/
```
**8. Copy and Paste on your NGROK Authtoken to your VPS**
- First login in : https://ngrok.com/ and regist with email
- go to `Your Authtoken` and Copy Paste `example command` on your web Ngrok
```
ngrok config add-authtoken 2v7axxxxxxxx
```
**`Next Command`**
```
ngrok http 3000
```
**After this you see `Forwarding` Copy `https://505xxxxxx.ngrok-free.app` to your Browser and Login with gmail**

**9. Next Submit your gmail and put `Code` in gmail**

`Would you like to push models you train in the RL swarm to the Hugging Face Hub? [y/N] N`

- If you see this , Done for run and go to home screen your VPS `CTRL+A+D`

![image](https://github.com/user-attachments/assets/78dd7960-f2d7-48d8-826b-9cdef3345ac4)
