# healthcare-blockchain-dapp
Blockchain-Based Healthcare Record System A decentralized healthcare management application built using Solidity, Web3.js, and React. This system enables secure patient record storage, consent-based access for doctors, and doctor rating features—all recorded on the Ethereum blockchain for transparency and immutability.


# Blockchain-Based Healthcare Record System

A decentralized healthcare record management system built using **Solidity**, **Ethereum**, and **Web3.js**, enabling secure storage, controlled access, and transparent interactions between **patients** and **doctors**.

---

## 🚀 Features

- **Patient & Doctor Registration**  
  Users can register as either patients or doctors with unique IDs.

- **Consent Management**  
  Patients explicitly grant or revoke access to doctors for their medical records.

- **Medical Record Management**  
  Doctors can add, update, and manage health records based on patient consent.

- **Doctor Ratings**  
  Patients can rate doctors on a 1–5 scale; ratings are averaged and publicly accessible.

- **Visibility Control**  
  Doctors can toggle visibility of individual records.

- **Secure Access**  
  Access to functions is tightly controlled using Solidity **modifiers** and **mappings**.

---

## 🛠 Tech Stack

| Layer         | Tech Used                           |
|---------------|-------------------------------------|
| **Frontend**  | HTML, CSS, JavaScript (Vanilla)     |
| **Library**   | Web3.js                             |
| **Smart Contract** | Solidity (Ethereum Blockchain) |
| **Development** | Hardhat / Remix / MetaMask        |

---

## 📦 Smart Contract Overview

- Written in **Solidity (v0.8.19)**
- Includes:
  - `registerPatient`, `registerDoctor`
  - `giveConsent`, `hasGivenConsent`
  - `addRecord`, `updateRecord`, `toggleRecordVisibility`
  - `giveRating`, `getDoctorRating`
  - `getRecords`, `getMyRecords`, `getRecordsPaginated`


---

## ⚙️ Getting Started

### Prerequisites

- [MetaMask](https://metamask.io/)
- [Node.js & npm](https://nodejs.org/)
- [Ganache](https://trufflesuite.com/ganache/) or testnet like Goerli
- [Remix IDE](https://remix.ethereum.org/) or Hardhat (optional)

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/CHANDANASHIVARUDRAPPA/healthcare-blockchain-dapp.git
   cd healthcare-blockchain-dapp
   ```

2. **Install Dependencies**
   If using local dev tools:
   ```bash
   npm install
   ```

3. **Deploy Contract**
   - Use Remix or Hardhat to compile and deploy `HealthRecord.sol`.
   - Copy the contract address and update it in `script.js` and frontend files.

4. **Run Frontend**
   Open `index.html` in a browser with MetaMask enabled.

---

## 🧪 Usage Guide

1. **Connect Wallet** via MetaMask.
2. Choose role: **Doctor** or **Patient**.
3. Register with a unique ID.
4. Patients:
   - Give/revoke consent to doctors.
   - Rate doctors.
   - View all personal records.
5. Doctors:
   - Add/update records for patients (only with consent).
   - View patient records if consented.

---

## ✅ Smart Contract Highlights

- **Structs:** `Doctor`, `Patient`, and `Record` store complex data.
- **Mappings:** Fast lookup for consents, registrations, and roles.
- **Access Control:** Enforced using `onlyDoctor` and `onlyPatient` modifiers.
- **Event Logging:** Every major action emits an event for transparency.
- **Gas Optimization:** Pagination used for large record fetches.

---


## 🙌 Acknowledgements

- Solidity & Ethereum Docs  
- OpenZeppelin Community  
- MetaMask & Web3.js Teams



