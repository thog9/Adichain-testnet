# ADI PredictStreet Bot Scripts 🚀

This collection of Python scripts automates task completion on the ADI PredictStreet platform — a Web3 prediction marketplace where users earn points by completing social tasks, opening packs, connecting wallets, and linking Twitter/X accounts.

🔗 Website: [AdiChain Testnet](https://sprint.adipredictstreet.com?referral_code=ADI-VV4DW-H2VMS-7XNZV)

---

## ✨ Features Overview

### General Features

- **Multi-Account Support**: Reads Twitter tokens from `tokenX.txt` to process multiple accounts in parallel.
- **Central Menu System**: Interactive menu for easy script selection via `main.py`.
- **Colorful CLI**: Uses `colorama` for visually appealing output with box-drawing borders and colored icons.
- **Asynchronous Execution**: Built with `asyncio` for efficient concurrent task processing.
- **Error Handling**: Comprehensive error catching with retry logic for API failures.
- **Bilingual Support**: Supports both English and Vietnamese output.
- **Proxy Support**: Supports SOCKS5 proxies via `proxies.txt`.

---

### Included Scripts

✨ **Auto Quest** (`quest.py`)

- ✅ Automatic quest listing & completion
- ✅ Twitter Like, Retweet, Tweet actions
- ✅ Telegram channel self-attestation
- ✅ Auto-skip on-chain / 3rd party quests (avoid 429)
- ✅ Smart 10-20s random delay between quests
- ✅ Points balance display (before/after)
- ✅ Multi-account parallel execution
- ✅ Proxy support

✨ **Check-In / Login X** (`checkin.py`)

- ✅ Twitter (X) OAuth2 login
- ✅ Daily check-in
- ✅ Session validation
- ✅ Multi-account support
- ✅ Proxy support

✨ **Open Daily Packs** (`pack.py`)

- ✅ Check available packs (daily & bonus)
- ✅ Auto open all available packs
- ✅ Reward parsing (points, multipliers, tickets, badges)
- ✅ Streak info display
- ✅ Multi-account support
- ✅ Proxy support

✨ **Connect Twitter** (`connect.py`)

- ✅ X (Twitter) account linking via OAuth2 PKCE
- ✅ Country setup & ADI Card generation
- ✅ Quest auto-completion
- ✅ Check-in & rewards balance
- ✅ Session validation
- ✅ Proxy & multi-threading support

✨ **Connect Wallet** (`connect-wallet.py`)

- ✅ Multi-chain wallet connection (POLYGON, BNB_CHAIN, ARBITRUM, ETHEREUM, ADI)
- ✅ Interactive chain selection menu (arrow keys)
- ✅ SIWE (Sign-In with Ethereum) message signing
- ✅ Respects server maxWallets limit
- ✅ Skips already-connected chains
- ✅ Proxy support

✨ **Mint ADI Card** (`mint.py`)

- ✅ Automatic ADI Card minting
- ✅ Transaction hash display
- ✅ Multi-account + multi-wallet pairing
- ✅ Proxy support

---

## 🛠️ Prerequisites

Before running the scripts, ensure you have the following installed:

- **Python 3.8+**
- **pip** (Python package manager)
- **Dependencies**: Install via `pip install -r requirements.txt`
- **tokenX.txt**: Add Twitter auth tokens (one per line, format: `auth_token|ct0`)
- **pvkey.txt** (optional): Add private keys for wallet operations
- **proxies.txt** (optional): Add SOCKS5 proxy addresses

---

## 📦 Installation

1. **Clone or download this repository:**
   ```sh
   git clone https://github.com/thog9/Adichain-testnet.git
   cd Adichain-testnet
   ```

2. **Install Dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Prepare Input Files:**

   Create `tokenX.txt` in the root directory with Twitter tokens (one per line):
   ```
   auth_token_value|ct0_value
   auth_token_value|ct0_value
   ```

   Create `proxies.txt` (optional) — one proxy per line (format: `ip:port:user:pass`):
   ```
   http://user:pass@ip:port
   socks5://user:pass@ip:port
   ```

   Create `pvkey.txt` (optional) — private keys for wallet/mint operations:
   ```
   0x999...
   0x999...
   ```

4. **Run:**
   ```sh
   python main.py
   ```
   - Choose a language (Vietnamese / English).
   - Select the script you want to run.

**Language Selection:**
- Choose between Vietnamese (Tiếng Việt) and English.
- All scripts support bilingual output.

---

## 📁 Project Structure

```
Adichain-testnet/
├── main.py                 # Central menu system
├── tokenX.txt              # Twitter auth tokens
├── pvkey.txt               # Private keys (optional)
├── proxies.txt             # SOCKS5 proxies (optional)
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── scripts/                # Individual scripts
    ├── quest.py            # Auto quest completion
    ├── checkin.py          # Check-in / Login X
    ├── connect.py          # Twitter OAuth connection
    ├── pack.py             # Open daily packs
    ├── connect-wallet.py   # Multi-chain wallet connection
    └── mint.py             # Mint ADI Card

```

---

## 📨 Contact

Connect with us for support or updates:

- **Telegram**: [thog099](https://t.me/thog099)
- **Channel**: [CHANNEL](https://t.me/thogairdrops)
- **Group**: [GROUP CHAT](https://t.me/thogchats)
- **X**: [Thog](https://x.com/thog099)

---

## ☕ Support Us

Love these scripts? Fuel our work with a coffee!

🔗 BUYMECAFE: [BUY ME CAFE](https://buymecafe.vercel.app/)

🔗 WEBSITE: [BUY SCRIPTS](https://thogtoolhub.com/)
