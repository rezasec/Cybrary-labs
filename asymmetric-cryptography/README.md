# Asymmetric Cryptography

This lab demonstrates secure communication using public key cryptography in a Linux environment, simulating encryption and decryption between two users: `cybrary` and `sally`.

## Key Concepts
- **Asymmetric cryptography** uses two keys:
  - **Public key** --> encrypts 
  - **Private key** --> decrypts 
- ✅ Solves key distribution and management issues
- ❌ Slower than symmetric encryption
- Used in: HTTPS, email encryption, digital signatures, PKI

##  Lab Summary

### 🔑Key Generation
- Generated a private key with:
  ```bash
  openssl genpkey -algorithm rsa -out cybraryprivate.key
