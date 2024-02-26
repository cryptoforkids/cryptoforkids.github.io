# RSA asymetric encryption

The RSA encryption algorithm was a groundbreaking discovery in the world of cryptography, developed by Ron Rivest, Adi Shamir, and Leonard Adleman in 1977. This method was once the backbone of internet security, ensuring that digital communications and transactions were kept private. RSA works by using a pair of keys: a public key for encrypting messages and a private key for decrypting them. The strength of RSA lies in the difficulty of factoring large numbers into their prime components, a task that is easy to perform in one direction but incredibly challenging to reverse without the private key.

Although RSA was immensely popular and widely used for securing online communications, its prominence has somewhat diminished over time. This shift is due to the advent of newer, more efficient cryptographic algorithms that require less computational power and offer faster processing times, making them more suitable for the increasing volume of data transmitted over the internet today.

Despite these challenges, RSA remains a valuable tool for educational purposes. Its conceptual simplicity, rooted in basic mathematical principles, makes it an excellent example for introducing students to the concepts of encryption and decryption. Understanding RSA provides a solid foundation in cryptography, illustrating the core ideas of public and private keys and the mathematical underpinnings of secure communications.

If you want to encrypt a message using the RSA you just need to follow all of the steps of the RSA algorithm, detailed below.

1. **Select Two Prime Numbers:** Begin by choosing two large prime numbers, pp and qq. The size of these primes ensures the security of the encryption.
2. **Compute the Product nn:** Calculate n=p×qn=p×q. The number nn is used as the modulus for both the public and private keys. Its length, usually in bits, is the key length.
3. **Calculate Euler's Totient Function (ϕ(n)ϕ(n)):** This is calculated as ϕ(n)=(p−1)×(q−1)ϕ(n)=(p−1)×(q−1). This value is used in determining the public and private keys and is crucial for ensuring that the encryption and decryption processes are inverses of each other.
4. **Choose the Public Key Exponent ee:** Select an integer ee that is greater than 1 and less than ϕ(n)ϕ(n) such that ee and ϕ(n)ϕ(n) are coprime (i.e., their greatest common divisor is 1). This ee will be part of the public key.
5. **Determine the Private Key Exponent dd:** Calculate dd as the modular multiplicative inverse of ee modulo ϕ(n)ϕ(n). This means dd is the number that satisfies the equation ed≡1mod  ϕ(n)ed≡1modϕ(n). The value of dd is kept secret as the private key.
6. **Public and Private Keys:** The public key is the pair (e,n)(e,n), and the private key is the pair (d,n)(d,n).

## Encryption and Decryption

* **Encryption:** To encrypt a message mm, where mm is a number smaller than nn, compute the ciphertext cc using the public key (e,n)(e,n) as c=memod  nc=memodn.
* **Decryption:** To decrypt ciphertext cc back to the message mm, use the private key (d,n)(d,n) to compute m=cdmod  nm=cdmodn.

This process leverages the one-way nature of certain mathematical functions—easy to compute in one direction (encryption) but hard to reverse without the private key (decryption), making asymmetric encryption a powerful tool for secure communication.

## Example 

Let's walk through an example of using the RSA algorithm with real numbers. We'll use small numbers for simplicity, but keep in mind that real-world applications use much larger primes to ensure security.

### Step-by-Step RSA Encryption and Decryption:

1. **Choose Two Prime Numbers:** For this example, we'll use _p=61_ and _q=53_.
2. **Calculate _n=p×q_:** Multiplying our primes, we get _n=3233_.
3. **Calculate Euler's Totient Function (_ϕ(n)_):** We calculate _ϕ(n)=(p−1)×(q−1)=3120_.
4. **Choose Public Key Exponent _e_:** We've chosen _e=17_, which is a common choice for small examples and is coprime with _ϕ(n)_.
5. **Determine Private Key Exponent _d_:** Calculating the modular multiplicative inverse of **e modulo ϕ(n)**, we find _d=2753_.

So, our public key is _(e,n)=(17,3233)_ and our private key is _(d,n)=(2753,3233)_.

### Encrypting a Message

Suppose our message _m_ is the number _123_. We encrypt it using our public key:

_c = m<sup>e</sup> mod n_
_c = 123<sup>17</sup> mod 3233_
_c = 

The final result is our ciphertext c.

### Decrypting the Message

Given our ciphertext _c_, we can decrypt it using our private key to recover mm:

_m=cdmod_

Let's perform these calculations to see the encryption and decryption in action. ​

​

After applying the RSA encryption and decryption steps with our example numbers, here's what happens:

    Encryption: The message m=123m=123 is encrypted using the public key (e,n)=(17,3233)(e,n)=(17,3233), resulting in the ciphertext c=855c=855.

    Decryption: The ciphertext c=855c=855 is decrypted back into the original message m=123m=123 using the private key (d,n)=(2753,3233)(d,n)=(2753,3233).

This process demonstrates how RSA encryption allows for secure communication, ensuring that only the holder of the private key can decrypt the message sent using the public key. In real-world applications, the numbers involved are significantly larger, making the encryption practically impossible to break with current technology.
