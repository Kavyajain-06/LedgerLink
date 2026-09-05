# 💳 LedgerLink AI — Trust Travels Even When Networks Don't

> **An AI-powered Offline-First FinTech Payment Platform built for resilient digital payments in low-connectivity environments.**

LedgerLink AI is a hackathon project that reimagines digital payments for situations where internet connectivity is unreliable or unavailable. Instead of depending on banking servers during payment authorization, LedgerLink AI enables customers and merchants to complete secure offline transactions using AI, cryptographic payment vouchers, local peer-to-peer communication, and deferred blockchain settlement.

---

## 🌍 Problem Statement

Digital payment systems like UPI and QR payments require continuous internet connectivity for authentication and verification. In rural areas, disaster zones, crowded events, mountainous regions, and network-congested locations, transactions often fail despite customers having sufficient funds and merchants having valid QR codes.

LedgerLink AI bridges this reliability gap by allowing payments to be **authenticated, verified, transferred, and stored locally**, then synchronized once internet connectivity returns.

---

## ✨ Key Features

### 👤 Customer Experience

* 🎙️ Offline Voice Payments using AI-powered speech recognition.
* 📷 QR Payments through **Camera** or **Gallery Upload**.
* 🧾 AI Receipt Scanner with OCR-generated digital invoices.
* 👥 AI Split Bill generation for group payments.
* 📊 AI Spending Insights with interactive analytics.
* 📜 Smart Transaction History with voucher and receipt tracking.

### 🏪 Merchant Experience

* 📥 Receive offline payment vouchers in real time.
* ✅ Verify cryptographic vouchers locally.
* 💾 Maintain an append-only SQLite transaction ledger.
* ⛓️ Monitor settlement queue.
* 📈 Merchant analytics dashboard.

### 🌐 Offline Payment Engine

* Offline-first payment workflow.
* Local Wi-Fi / LAN voucher transfer.
* Cryptographically signed payment vouchers.
* Deferred blockchain settlement.
* Connectivity simulator (Offline • LAN Connected • Internet Connected).

---

## 🏗️ System Architecture

LedgerLink AI follows a layered offline payment architecture.

| Layer                     | Responsibility                                                                 |
| ------------------------- | ------------------------------------------------------------------------------ |
| **AI Intelligence Layer** | Offline voice recognition, intent parsing, OCR receipt extraction.             |
| **Authentication Layer**  | WebAuthn biometric authentication using Passkeys.                              |
| **Cryptographic Layer**   | EIP-712 signed payment voucher generation.                                     |
| **Transport Layer**       | Peer-to-peer voucher transfer over Wi-Fi/LAN.                                  |
| **Local Ledger Layer**    | SQLite append-only storage for pending transactions.                           |
| **Settlement Layer**      | Synchronization and settlement on Monad blockchain after connectivity returns. |

---

## 🔄 End-to-End Payment Pipeline

1. User initiates payment via **Voice**, **QR**, or **Manual Entry**.
2. AI extracts payment intent locally.
3. User authenticates with **WebAuthn** (Fingerprint / Face ID / Windows Hello).
4. LedgerLink generates an **EIP-712 cryptographically signed voucher**.
5. Voucher is transferred directly to the merchant over a **local Wi-Fi/LAN connection**.
6. Merchant verifies and stores the voucher in a **SQLite ledger**.
7. When internet connectivity returns, vouchers are synchronized through a settlement queue and confirmed on the **Monad blockchain**.

---

## 🔐 Security & Trust Mechanisms

LedgerLink AI preserves transaction integrity even in offline mode.

* **WebAuthn Passkeys** for passwordless biometric authentication.
* **Secure Enclave** for on-device private key protection.
* **EIP-712 Typed Data Signing** for tamper-proof payment vouchers.
* **Nonce-Based Replay Protection** to prevent duplicate transactions.
* **Expiry Timestamps** for voucher validity.
* **Offline Signature Verification** by merchants before accepting payments.
* **Append-Only SQLite Ledger** for immutable offline transaction storage.
* **Blockchain Settlement Integrity** once connectivity is restored.

---

## 🤖 AI Features

### Offline AI Voice Payments

* Local speech recognition.
* Real-time transcript generation.
* Intent extraction for merchant and amount.
* Confidence score simulation.

### AI Receipt Scanner

* Camera capture or gallery upload.
* OCR-based receipt parsing.
* Merchant and GST extraction.
* Automatic digital invoice generation.

### AI Spending Insights

* Weekly and monthly spending analytics.
* Category-wise expense visualization.
* Merchant frequency tracking.
* Offline vs settled transaction insights.

---

## 📱 Customer Dashboard

The customer dashboard includes:

* Wallet Balance.
* Offline Spending Capacity.
* Pending Settlements.
* Voice Pay.
* QR Pay.
* Split Bill.
* Receipt Scanner.
* Transaction History.
* AI Spending Insights.

---

## 💻 Merchant Dashboard

The merchant dashboard includes:

* Today's Revenue.
* Pending Offline Payments.
* Voucher Verification Queue.
* SQLite Ledger Explorer.
* Settlement Center.
* Merchant Analytics.
* Live Incoming Payment Notifications.

---

## 🎭 Prototype Experience

This project is deployed as a **frontend-only interactive prototype** on **Netlify**.

### Simulated Components

* AI speech recognition.
* WebAuthn biometric authentication.
* QR camera scanning.
* Gallery QR upload.
* Receipt OCR extraction.
* Voucher generation.
* Peer-to-peer Wi-Fi transfer.
* SQLite ledger updates.
* Monad blockchain settlement.
* Network connectivity changes.

Everything is powered through **mock APIs**, **synthetic data**, and **frontend state management**.

---

## 📊 Synthetic Demo Data

The prototype launches with realistic demo data.

* 20 Customer profiles.
* 12 Merchant profiles.
* 60+ Transaction records.
* AI-generated receipts.
* Pending and settled vouchers.
* QR codes for merchants.
* Wallet balances.
* Notifications.
* Spending analytics.

Every payment dynamically updates balances, ledgers, settlement queues, and analytics.

---

## 🛠️ Tech Stack

### Frontend

* React
* Tailwind CSS
* React Router
* Framer Motion (animations)

### AI Simulation

* Moonshine ONNX (offline speech recognition concept)
* OCR simulation
* Intent parsing simulation

### Security Concepts

* WebAuthn Passkeys
* Secure Enclave
* EIP-712 Typed Data Signing

### Data Layer

* SQLite (simulated local ledger)
* Browser Local Storage (prototype persistence)

### Blockchain

* Monad Testnet settlement simulation

### Deployment

* Netlify

---

## 🚀 Demo Workflow

1. Open LedgerLink AI.
2. Select **Customer** or **Merchant** role.
3. Authenticate using simulated biometrics.
4. Make an offline payment using Voice or QR.
5. Watch voucher arrive on the Merchant Dashboard.
6. View transaction stored in SQLite ledger.
7. Simulate internet reconnection.
8. Watch vouchers settle on Monad blockchain.

---

## 💡 Innovation

LedgerLink AI is not another payment application—it is an **offline payment resilience platform**.

Unlike conventional UPI systems that require online authorization, LedgerLink AI establishes trust locally using cryptographically signed payment vouchers, peer-to-peer communication, local ledger storage, and deferred blockchain settlement.

The platform combines **AI, cryptography, offline networking, and blockchain** into a seamless customer and merchant payment ecosystem.

---

## 👥 Future Scope

* Real Moonshine ONNX speech model integration.
* Actual WebAuthn implementation.
* SQLite + Express backend.
* Wi-Fi Direct communication.
* Real Monad smart contract deployment.
* Multi-language offline AI assistant.
* Merchant POS integration.
* Disaster-relief offline payment network.

---

## 📄 License

This project was built as a hackathon prototype for educational and demonstration purposes.
