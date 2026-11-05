# Blockchain-Based Product Identification System

Project Overview
The Blockchain-Based Product Identification System is a web-based application designed to ensure product authenticity, transparency, and security using blockchain technology. It helps users identify and verify genuine products while preventing counterfeit products and unauthorized modifications.

The system uses blockchain to securely store product information and maintain a tamper-resistant record of product registration and ownership transfers. Each product is assigned a unique QR code that allows users to easily access and verify its details.

Key Features
- **Product Registration:** Register products with details such as product name, manufacturer, category, origin, and manufacturing date.
- **Blockchain Integration:** Store product data hashes on the blockchain to ensure data integrity and prevent unauthorized modifications.
- **QR Code Generation:** Generate unique QR codes for registered products.
- **Product Verification:** Scan QR codes to verify product authenticity and retrieve product information.
- **Ownership Transfer:** Securely transfer product ownership and maintain transaction records.
- **Tamper Detection:** Verify product information against blockchain records to identify unauthorized changes.
- **Web-Based Interface:** User-friendly frontend for product registration, identification, and verification.

Technologies Used
- **Frontend:** React.js, Vite, JavaScript, HTML, CSS
- **Backend:** Python, Django, Django REST Framework
- **Blockchain:** Ethereum, Solidity, Hardhat
- **Blockchain Library:** Web3.py
- **QR Code:** QR Code Generation and Scanning
- **Database:** Django-supported database
- **Development Tools:** Visual Studio Code, Node.js

 System Workflow
1. The manufacturer registers a product through the web application.
2. Product details are stored in the backend.
3. A unique hash of the product information is generated using SHA-256.
4. The hash is registered on the Ethereum blockchain through a smart contract.
5. A unique QR code is generated for the product.
6. Users scan the QR code to retrieve product details.
7. The system verifies the product information against the blockchain record.
8. Ownership can be transferred securely, with the transaction recorded on the blockchain.

Project Objective
The main objective is to develop a secure and transparent product identification system that builds trust between manufacturers, distributors, retailers, and customers by using blockchain technology.

Future Enhancements
- Integration of IoT devices for real-time product tracking.
- Email and SMS notifications.
- Deployment on a public blockchain network.
- Advanced product supply-chain tracking.
- Mobile application integration.

Conclusion
This project demonstrates how blockchain technology can be used to improve product identification, authentication, and traceability. By combining blockchain, smart contracts, QR codes, and web technologies, the system provides a reliable approach to reducing counterfeit products and improving supply-chain transparency.
