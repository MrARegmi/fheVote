# Quantum-Resistant Decentralized Voting System

A secure, decentralized voting application that uses fully homomorphic encryption (FHE) and IPFS storage. This project integrates a frontend UI, a backend API, smart contracts on an Ethereum network, and a Golang microservice for data aggregation.

## Features

- **Frontend**:

  - React.js and TypeScript for a dynamic user interface.
  - Web3.js or Ethers.js to interact with blockchain smart contracts.
  - Registration, Voting, and Results pages.

- **Backend**:

  - Node.js with Express.js for API endpoints.
  - PostgreSQL/MongoDB for data storage and Redis for caching.
  - Fully Homomorphic Encryption (FHE) for data security.

- **Blockchain**:

  - Solidity smart contracts for voter registration and voting.
  - OpenZeppelin libraries for access control and secure contract patterns.

- **Microservice**:

  - Golang microservice for encrypted data aggregation.

- **IPFS Storage**:
  - Secure, decentralized storage for encrypted vote data.

## Architecture

Frontend (React and TypeScript):
Imagine a bright, interactive user interface built with React and TypeScript.
Three primary sections (registration, voting, and results) are the gateways through which users interact.
Encrypted data flows directly into a Web3.js or Ethers.js pipe, securely connecting to the blockchain smart contracts.
Backend (Node.js and Express.js):
Visualize a busy command center: Express.js handles secure API endpoints, relaying data to and from the blockchain, IPFS, and microservices.
PostgreSQL and MongoDB databases serve as vaults for storing user data, while Redis acts as a memory cache for frequently accessed results.
The backend securely manages Fully Homomorphic Encryption (FHE) operations, shielding sensitive data with cryptographic armor.
Blockchain Smart Contracts (Solidity):
Picture a fortified ledger on the Ethereum blockchain, where smart contracts serve as guards at the gate:
A Voter Registry secures the perimeter, registering only authorized voters.
A Voting Contract records encrypted vote data with a cryptographic seal, emitting events for tallying.
Golang Microservice:
Envision a swift and efficient data aggregator:
Fetching encrypted data from IPFS using CIDs provided by the backend.
Tallying votes using FHE, the microservice returns aggregated, anonymized results.
IPFS Storage:
Think of a digital library with secure vaults scattered across a peer-to-peer network.
Encrypted votes and sensitive user data are neatly stored and accessible by unique content identifiers (CIDs).
Data Flow:
Frontend to Backend: User registration and voting data flow securely from the frontend to the backend.
Backend to Smart Contracts: Verified data is sent to blockchain smart contracts.
Backend to IPFS: Data is encrypted, stored in IPFS, and retrieved by its CID.
Golang Microservice Aggregation: Aggregated data flows back to the backend and the frontend to display results.

## Getting Started

### Prerequisites

- Node.js
- Docker
- Golang
- An Ethereum wallet (e.g., MetaMask)
- IPFS client or gateway access
