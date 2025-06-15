# 🔐 Symmetric Cryptography

This lab demonstrates how symmetric encryption works in practice using a shared secret key between two users in a Linux environment.

## Key Concepts
- Symmetric encryption which uses the same key for both encryption and decryption.
- It’s fast and ideal for large data encryption 
- Key sharing is the challenge
- Doesn’t scale well with many users 

## Lab Summary
Simulated secure communication between two Linux users:

- **User cybrary** created a secret key and sent it to john using base64 encoding + local email.
- **John**
  - Received the key.
  - Composed a secret message.
  - Encrypted it using the shared key with `openssl pkeyutl`.
  - Sent it back to cybrary in base64.
- **Cybrary**
  - Decoded the message.
  - Decrypted it using the same shared key.

## Tools Used
- `openssl` for key generation, encryption, decryption
- `base64` for encoding/decoding messages
- `mail` for local email transmission

## Key Takeaway
Symmetric encryption is simple and powerful but securely sharing and managing keys at scale is a real world limitation.
