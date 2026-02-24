# Bitcoin Ordinals Indexer

An essential tool for developers building on Bitcoin's Layer 1. This indexer tracks the movement of individual satoshis and extracts inscription data (images, text, JSON) to provide a clean API for NFT marketplaces or wallet explorers.

## Features
* **Sat Tracking:** Logic to track satoshis across inputs and outputs (FIFO).
* **Metadata Extraction:** Automatically parses hex data from witness fields to reconstruct inscriptions.
* **Electrum Integration:** Uses low-latency Electrum servers for real-time mempool and block monitoring.
* **SQLite Persistence:** Stores indexed inscriptions in a local, lightweight database for fast querying.

## Prerequisites
* Node.js (v18+)
* Access to a Bitcoin Node or public Electrum server.

## Installation
1. `npm install`
2. Update `config.js` with your Electrum server details.
3. Start indexing: `node indexer.js`
