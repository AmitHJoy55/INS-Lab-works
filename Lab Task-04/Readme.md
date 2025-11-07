# Lab - 4 : Programming Symmetric & Asymmetric Crypto

✨[**Notebook Link**](Lab_4.ipynb)

### 🎯 Objectives  
- To **program symmetric and asymmetric cryptography** operations.  
- To **measure and study execution time** for various cryptographic functionalities.  
- To gain a deeper understanding of how cryptographic mechanisms operate beyond built-in tools like `openssl`.

---

### 🧩 Implemented Functionalities  

The program provides a **menu-driven interface** to perform multiple cryptographic operations, similar to OpenSSL:

1. **AES Encryption**
2. **AES Decryption**
3. **RSA Encryption**
4. **RSA Decryption**
5. **RSA Signature Generation**
6. **RSA Signature Verification**
7. **SHA-256 Hashing**
8. **Exit**

#### AES Operations  
- Supports **128-bit** and **256-bit** key lengths.  
- Two modes implemented: **ECB** and **CFB**.  
- Encrypted data is stored in a file, which is later decrypted and printed on the console.  

#### RSA Operations  
- RSA **key pair generation** at program start.  
- RSA **encryption and decryption** of plaintext.  
- **RSA Signature** generation for a file and verification using a separate signature file.

#### SHA-256 Hashing  
- Generates a SHA-256 hash of an input file or data and displays it on the console.

### Example Execution:

- Enter choice: 1
- Enter AES key length (128 or 256): 128
- Enter AES mode (ECB or CFB): ECB
- Enter data to encrypt: Deep Learning is fascinating!
- AES encryption took 0.01109623908996582 seconds

#### Execution Time Measurement  
- The program measures and displays the **execution time** for each cryptographic operation.  
- Performance was analyzed with **five different key sizes (starting from 16 bits)** for both AES and RSA.  
- Graphs were plotted to show **time vs. key size** and included in the report.

---
| Operation        | Key Size (bits) | Avg Time (s) |
| ---------------- | --------------- | ------------ |
| AES Encryption   | 128             | 0.0111       |
| AES Decryption   | 128             | 0.0013       |
| RSA Encryption   | 2048            | 0.0014       |
| RSA Decryption   | 2048            | 0.0017       |
| RSA Signature    | 2048            | 0.0029       |
| RSA Verification | 2048            | 0.0004       |
| SHA-256 Hashing  | —               | 0.0011       |


## Resources

- [Cryptography.io](https://cryptography.io/en/latest/)
- [Laurent Luce's Blog](https://www.laurentluce.com/posts/python-and-cryptography-with-pycrypto/)