# CLI Node Run Full Guide (PC and VPS for Both)

Go to: https://app.hyperbolic.xyz

- Click Create Account by Using ur Gmail
- On next popup or in Settings, confirm ur phone number to get 1$ of free credits (Compulsory)
- Go to Settings tab on Hyperbolic dashboard > Scroll down and copy ur API Key

1️⃣ Dependencies for WINDOWS & LINUX & VPS
```
sudo apt update && sudo apt upgrade -y
```

2️⃣ Install Python & Pip
```
sudo apt install git python3 python3-pip python3-venv -y
```

3️⃣ Download Some Files
```
git clone https://github.com/0xmoei/chatbot-app.git
cd chatbot-app
```

For VPS Only
```
apt install screen -y
```
```
screen -S hyperbolic
```

4️⃣ Install these Python Pre-Requisites
```
python3 -m venv venv
source venv/bin/activate
pip install requests
```

5️⃣ Configure Environment Variables
```
nano chatbot.py
```
Then Save Press CTRL+X, then Y, then Enter
- Edit the "Authorization" line & Replace ur 'YOUR_API_KEY_HERE' with your actual API key u got already.

6️⃣ Start Node
```
python3 chatbot.py
```
- Once it reaches the 100-question limit, it will stop automatically. To resume, simply use the **Start Node** command again.

For VPS Only
```
PRESS CTRL+A+D (to run ur node continuously)
```
- To check ur Node Again
```
screen -r hyperbolic
```

## 🔶For Next Day Run This Command

#1 Open WSL and Put this Command 
```
cd chatbot-app
```
```
python3 chatbot.py
```
