# 🔐 PassStrengthX

PassStrengthX is a powerful Python-based CLI tool that checks the **strength of a password** using entropy calculation and Dropbox's `zxcvbn` estimation. It also verifies whether the password has been exposed in known **data breaches** via the HaveIBeenPwned API — all using privacy-preserving techniques.

---

## 🚀 Features

- 🧠 Calculates password entropy in bits  
- 📊 Classifies password strength: Very Weak to Very Strong  
- 🔍 Checks if the password exists in public data breaches (using k-Anonymity)  
- 💻 Simple CLI usage — cross-platform  
- 🔒 Works offline except for breach checking

---

## 🛠 Usage

1. Clone the repo and enter the directory  
2. Set up a virtual environment (recommended)  
3. Install dependencies from `requirements.txt`  
4. Run:

```bash
python3 passstrengthx.py --password "YourPasswordHere"

Example:
python3 passstrengthx.py --password "Cyber@Dharmik2025"

🔐 Checking password: Cyber@Dharmik2025

🧠 Entropy: 111.43 bits  
📊 Strength: 🟦 Very strong  
✅ Not found in known breaches.

📁 Project Structure
graphql
Copy code
passstrengthx/
├── passstrengthx.py          # Main CLI tool logic
├── requirements.txt          # Dependencies
├── utils/
│   └── entropy.py            # Entropy calculator module
└── README.md                 # You're reading it

📦 Requirements
zxcvbn – For estimating password strength

requests – For API calls to HaveIBeenPwned

Install them with:

bash
Copy code
pip install -r requirements.txt
🧠 Entropy Reference Table
Entropy (bits)	Strength Level
0–28	🔴 Very Weak
29–35	🟠 Weak
36–59	🟡 Moderate
60–127	🟦 Strong
128+	🟩 Very Strong

👨‍💻 Author
Dave Akshat
🔗 GitHub: https://github.com/Akshatraja


