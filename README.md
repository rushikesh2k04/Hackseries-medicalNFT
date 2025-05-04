🏥 Medical NFT – Prescription as a Token
Medical NFT is a decentralized platform that enables doctors to mint verifiable prescriptions as Non-Fungible Tokens (NFTs) on the Algorand blockchain. It ensures secure, tamper-proof, and traceable prescription delivery using smart contracts written in PyTeal, with frontend integration using algosdk.

🚀 Features
✅ Doctor Verified NFT Minting

Each prescription is minted as an NFT (Algorand Standard Asset)

Includes:

Asset name, title, description

PDF link of the signed prescription

Patient's wallet address

Total supply of 1, zero decimals (indivisible)

✅ Secure IPFS Storage

Prescriptions are uploaded to IPFS (e.g., via Pinata)

IPFS hash is embedded in the ASA metadata

✅ NFT Transfer to Patient

Automatically sent to the patient’s wallet after minting

✅ Immutable Medical Records

On-chain, tamper-proof record of prescriptions

Doctor identity verification supported 

✅ ARC-3 Compliant

Compatible with major Algorand wallets for seamless access and sharing

🔗 Workflow
Doctor Login
Doctors connect their wallet or log in via organization credentials

Prescription Upload
Doctors enter the title, description, upload the signed PDF, and specify the patient’s wallet address

NFT Minting
PDF is uploaded to IPFS → Metadata is embedded → NFT is minted on Algorand

NFT Transfer
The prescription NFT is automatically transferred to the patient’s wallet

Patient Access
Patients can view, download, or share the prescription from their wallet

💻 Technologies Used
Layer	Technology
Blockchain	Algorand
Smart Contract	PyTeal
ABI Interface	ARC3
NFT Minting	algosdk
Wallets	Pera Wallet, Defly Wallet, Exodus Wallet, Daffi Wallet
File Storage	IPFS / Pinata
Frontend	React.js + algosdk
Security	Wallet Auth

📂 Project Structure
bash
Copy
Edit
/medicalnft-contracts
  └── medinft/contract.py       # Smart contract in PyTeal
/medicalnft-frontend
  └── src                       # NFT minting logic
        └── pages
            └── MarkeplacePage.tsx
            └── MedicalservicesPage.tsx
        └── Home.tsx
        └── App.tsx                   # Main UI for doctors and patients
🧠 Smart Contract Functions
Function	Description
create_prescription(asset_metadata)	Mint a prescription NFT and send to patient
delete_prescription()	Allow deletion of invalid or expired records (if applicable)

🛠 Prerequisites
Python + PyTeal for smart contract development

Node.js + algosdk for frontend

Testnet ALGO from Algorand Faucet

Wallet setup (Pera Wallet, Defly Wallet, etc.)

IPFS storage setup (Pinata, Web3.Storage)

📦 Installation & Setup
bash
Copy
Edit
# Clone the repository
git clone https://github.com/rushikesh2k04/Hackseries-medicalNFT.git
cd projects

Doctor dashboard with prescription history

Patient dashboard with NFT viewer and access logs

Expiry dates or revocation mechanism for prescriptions

Integration with pharmacy APIs for direct order placement

✨ Author
Rushikesh – Blockchain Developer,FullStack
Connect: rushikesh9.2004@gmail.com

💡 Inspiration
Medical NFT leverages blockchain’s transparency and immutability to redefine how prescriptions are issued and managed. It ensures that patients receive secure, verifiable medical records while giving doctors a modern, tamper-proof platform for prescription management.

