#bridge 

The study of techniques for secure communication, ensuring confidentiality, integrity, authentication, and non-repudiation of data.

### Classical Cryptography

- **Caesar cipher:** Shift each letter by a fixed amount in the alphabet.
- **Vigenère cipher:** Use a repeating key to apply different shifts.
- **Substitution cipher:** Replace each symbol with another symbol.
- **Transposition cipher:** Rearrange symbols without changing them.

---
### Modern Cryptography

Uses mathematical algorithms, often based on [[Number theory]], for stronger security.
#### Symmetric-key encryption
- The same key is used for both encryption and decryption.
- Examples: AES (Advanced Encryption Standard), DES (Data Encryption Standard).
- Fast but requires secure key sharing.
#### Asymmetric-key encryption (Public-key)
- Uses a public key for encryption and a private key for decryption.
- Based on hard problems like prime factorization or discrete logarithms.
- Examples: RSA, ElGamal, ECC (Elliptic Curve Cryptography).

---
#### Hash Functions
- A hash maps data of arbitrary size to a fixed-size output.
- Properties: one-way (hard to invert), collision-resistant.
- Examples: SHA-256, SHA-3, MD5 (obsolete).

---
#### Digital Signatures
- Provide authentication and integrity.
- A private key signs a message, and a public key verifies it.
- Examples: RSA signatures, ECDSA.

---
#### Key Exchange
- Protocols for securely sharing keys over insecure channels.
- Example: Diffie-Hellman key exchange.

---
#### Applications
- Secure communications (TLS, HTTPS)
- Password storage (hashing + salting)
- Blockchain and cryptocurrencies
- Digital certificates and PKI

---
#### Attacks and Security
- Brute force: Trying all keys.
- Cryptanalysis: Exploiting weaknesses in algorithms.
- Side-channel attacks: Using timing, power consumption, or other physical leaks.

[[Cybersecurity]]
[[Quantum computing]]
