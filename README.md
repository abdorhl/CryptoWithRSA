# RSA Algorithm Proof in Python
A demonstration of the RSA algorithm in Python, featuring functions to generate key pairs, encrypt, and decrypt messages. This script illustrates the fundamental concepts of RSA, including prime number selection, modular arithmetic, and key pair generation.

# Overview
This project provides an end-to-end implementation of RSA encryption and decryption, with support for custom bit-length selection and message input. It demonstrates each step of the RSA process, from generating prime numbers to performing modular exponentiation for encryption and decryption.

**RSA Algorithm**
* Pick two large primes $p,q$.
* Compute $n=pq$ and $\varphi(n)=\mathrm{lcm}(p-1,q-1)$
* Choose a public key $e$ such that $1< e< \varphi(n)$ and $\gcd(e,\varphi(n))=1$
* Calculate $d$ such that $de\equiv 1 \pmod\varphi(n)$
* Let the message **key** be $m$
* **Encrypt: ** $c\equiv m^e\pmod n$
* **Decrypt: ** $m\equiv c^d\pmod n$

![Image Description](https://github.com/abdorhl/CryptoWithRSA/raw/main/imgs/rsa_system_algo.png)

# Example Output
Upon running the program, you’ll see the generated public and private keys, encrypted message, and decrypted message, similar to this:
![Image Description](https://github.com/abdorhl/CryptoWithRSA/raw/main/imgs/execute.png)

# Notes
This RSA implementation is designed for educational purposes and should not be used for real-world encryption.

For stronger encryption, use larger key sizes.

Note that you may have to setup an external dependency environment in some cases, it would create a big chunk of files that are not here due to exceeding the maximum number of files to upload.
