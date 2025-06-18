# Asymmetric Cryptography

In this lab, I explored the basics of public key cryptography using OpenSSL in a Linux environment. I started by generating a key pair, then published the public key so others could use it. From there, I practiced encrypting a message with another user’s public key and decrypting incoming messages with my own private key.

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

 
