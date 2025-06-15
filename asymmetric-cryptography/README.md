# Asymmetric Cryptography

This lab demonstrates how public key cryptography works using OpenSSL in a Linux environment. The process involved creating a key pair, publishing the public key, encrypting a message using another user’s public key, and decrypting a received message using a private key.

## Key Concepts
- Uses two keys: public (encrypt) and private (decrypt)
- Public keys can be shared. Private keys must remain secret
- Solves key distribution and management issues
- Common in HTTPS, email encryption, digital signatures

##  Lab Summary
- Generated RSA key pair: `cybraryprivate.key` and `cybrarypublic.key`
- Shared public key via simulated keyserver
- Downloaded `sallypublic.key` and encrypted a message to Sally
- Used base64 encoding to send message via mail
- Switched to Sally user, decoded, and decrypted message using `sallyprivate.key`

 
