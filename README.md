# QuantumChat

This project demonstrates a private and secure chat server using Quantum Key Distribution (QKD) for enhanced security. Clients connect to the server, perform QKD to establish a shared symmetric key, and communicate securely using this key.

## Prerequisites

- Python 3.6+
- `numpy` library (`pip install numpy`)
- `cryptography` library (`pip install cryptography`)

## Overview

The chat server uses the BB84 protocol from quantum cryptography to establish a shared symmetric key between the server and each client. Messages exchanged between clients and the server are encrypted and decrypted using this shared key, ensuring privacy and security.

## Project Structure

- `chat_server.py`: Server script that listens for client connections, performs QKD, and handles encrypted message exchange.
- `chat_client.py`: Client script that connects to the server, performs QKD with the server, and sends/receives encrypted messages.
- `bb84.py`: Module containing functions for BB84 key exchange and symmetric key generation.
- `README.md`: This file, providing an overview, prerequisites, and setup instructions.

## Setup and Usage

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/qkd-secure-chat.git
   cd qkd-secure-chat

2. **Install Dependencies**

   ```bash
   pip install numpy cryptography

3. **Run the Server**

   ```bash
   python chat_server.py

4. **Run the Client(s)**

   ```bash
   python chat_client.py

