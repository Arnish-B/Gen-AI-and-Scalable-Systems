# Gen-AI-and-Scalable-Systems
## Table of Contents
- [Astra DB Token Generation](#astra-db-token-generation)
- [NGROK Installation](#ngrok-installation)
  - [Windows Installation](#windows-installation)
  - [Linux Installation](#linux-installation)
  - [MacOS Installation](#macos-installation)
- [Changing Embedding Model Base URL](#changing-embedding-model-base-url)
- [Miscellaneous Links](#miscellaneous-links)
---
## Astra DB Token Generation
Follow these steps to generate your Astra DB token:
1. Navigate to the [Astra Datastax Dashboard](https://astra.datastax.com)
2. Create an account or sign in
3. Click **Create Database**
4. Select **Serverless (vector)** as the database type
5. Enter a name for your database
6. Select a cloud provider (Amazon Web Services recommended)
7. Select a region `us-east-2` recommended for AWS)
8. Click **Create Database**
9. Wait for the database status to change from "Pending" to "Active"
10. Generate a new token
11. **Important:** Store the token in a secure location for future use
---
## NGROK Installation
Visit the [NGROK website](https://ngrok.com) and create an account before proceeding with installation for your operating system.
### Windows Installation
1. Open the Microsoft Store
2. Search for **NGROK**
3. Install NGROK
4. Open Command Prompt or PowerShell and run:
```bash
   ngrok config add-authtoken 35QpgtvsHcNdLGPqLRUjErhPdAm_4jpziQBHHZwCdNLNNQoQq
```
5. Verify successful installation by running:
```bash
   ngrok http 80
```
### Linux Installation
1. Open your terminal
2. Install NGROK by running:
```bash
   curl -sSL https://ngrok-agent.s3.amazonaws.com/ngrok.asc \
     | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null \
     && echo "deb https://ngrok-agent.s3.amazonaws.com bookworm main" \
     | sudo tee /etc/apt/sources.list.d/ngrok.list \
     && sudo apt update \
     && sudo apt install ngrok
```
3. Add your authtoken to the default configuration:
```bash
   ngrok config add-authtoken 35QpgtvsHcNdLGPqLRUjErhPdAm_4jpziQBHHZwCdNLNNQoQq
```
4. Verify successful installation by running:
```bash
   ngrok http 80
```
### MacOS Installation
1. Install NGROK via Homebrew:
```bash
   brew install ngrok
```
2. Add your authtoken to the default configuration:
```bash
   ngrok config add-authtoken 35QpgtvsHcNdLGPqLRUjErhPdAm_4jpziQBHHZwCdNLNNQoQq
```
3. Verify successful installation by running:
```bash
   ngrok http 80
```
---
## Changing Embedding Model Base URL
1.
## Miscellaneous Links
1. [PPT](https://docs.google.com/presentation/d/1NGlG6n9ivMGOBnWePZs1M37HaE4-H9AHfe74d6kBXYQ/edit?usp=sharing)
2. [Langflow](https://www.langflow.org/)
3. [Astra DB](https://astra.datastax.com/)
4. [NGROK](https://ngrok.com/)
5. [CDN Animation](https://claude.ai/public/artifacts/2e7d90dd-c384-47f9-885b-2e71f95c369c)
6. [Data Sharding Animation](https://claude.ai/public/artifacts/7f4f061b-3c5f-4892-8cc7-1682653a5967)
7. [Scaling Animation](https://k8-sim-bmsce.netlify.app/)
