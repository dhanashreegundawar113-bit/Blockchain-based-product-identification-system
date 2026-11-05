# Blockchain-Based Product Identification System

A web-based product identification and verification application that combines a React frontend, Django REST backend, and an Ethereum-compatible blockchain smart contract. Products can be registered, identified using QR codes, verified against blockchain records, and transferred to a new owner.

## Features

- Product registration through a web interface
- SHA-256 hashing of selected product information
- Blockchain registration of product hashes
- QR code generation and scanning
- Product detail retrieval and verification
- Ownership transfer with blockchain transaction records

## Technology Stack

- **Frontend:** React, Vite, JavaScript
- **Backend:** Python, Django, Django REST Framework
- **Blockchain:** Solidity, Hardhat, Ethereum-compatible development network
- **Blockchain connection:** Web3.py
- **QR codes:** QR code generation and scanning

## Project Structure

```text
project-root/
├── README.md
├── .gitignore
├── backend/
│   ├── manage.py
│   ├── requirements.txt
│   ├── .env.example
│   ├── product_system/
│   └── products/
├── frontend/
│   ├── package.json
│   └── src/
└── blockchain/
    ├── contracts/
    ├── scripts/
    ├── hardhat.config.js
    └── package.json
```

> Keep your actual working folder structure if it differs from this example. Do not move or rename working files just to match this diagram.

## Prerequisites

- Python
- Node.js and npm
- A local Hardhat development node (for local development)

## Setup

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd Blockchain-Based-Product-Identification-System
```

### 2. Backend setup

```powershell
cd backend
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

Copy `.env.example` to `.env` and fill in your own local configuration values. Never commit `.env`.

Run database migrations and start Django:

```powershell
python manage.py migrate
python manage.py runserver
```

### 3. Blockchain setup

Open a separate terminal and navigate to the folder that contains your Hardhat `package.json` and `hardhat.config.js`.

Install dependencies:

```bash
npm install
```

Start your local Hardhat node and deploy your existing contract using the project's deployment script. Use the exact script and commands configured in your project.

Make sure the deployed contract address and ABI information used by the backend match the current local deployment. A local Hardhat chain resets when its node is restarted, so you may need to redeploy.

### 4. Frontend setup

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed by Vite in the terminal.

## Environment variables

Create `backend/.env` using `backend/.env.example` as a guide. Add your own local RPC URL, private key, and frontend URL. Never put a real private key, seed phrase, password, or API secret in GitHub.

## Security notes

- Never commit `.env` files or private keys.
- Use development-only accounts and keys on a local Hardhat network.
- Do not use a funded wallet's private key in this project.
- A public contract address and ABI are not private credentials, but verify that your contract information file contains no secrets before committing it.

## Important

This repository's README describes the intended setup. Check the actual scripts, dependency versions, environment variable names, and folder locations in your project before running commands. Update this document if your implementation differs.
