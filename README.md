# Getting started with cryptography

Modern cryptography is used by phones and computers to keep all of our digital information secret, safe and secure.  It's used everywhere, but most people don't know how it works or even what it does.

The funny thing is, the core algorithms underlying modern cryptography are built using  arithmatic and algebraic concepts that most middle-schoolers would be familiar with.  This website aims to teach the basic concepts of modern cryptography with that in mind.  After learning everything presented here, middle-school students should be able to hide and share secret messages using math that they already understand.

# What is Cryptography?
    
Cryptography is the science of encoding and decoding information to keep it secret and secure from unauthorized access. Throughout history, cryptography has played a crucial role in military and diplomatic communications, evolving from simple substitution ciphers used in ancient times to complex algorithms that protect our digital world today. 

The advent of computers and the internet in the 20th century transformed cryptography, leading to the development of modern cryptography. This era introduced computational algorithms that leverage mathematical theories to secure data, enabling everything from secure online transactions to private communications over the internet.

Modern cryptography gives us a set of mathematical tools that people can use to communicate without anyone else knowing what they're saying. Imagine you wrote a note that said, "Let's meet at the park at 4 PM," but you didn't want anyone else to know about it. With modern cryptography, you can scramble your message into something that looks like nonsense to anyone who finds it—unless they know the secret that allows them to decrypt the message.  Modern cryptography also gives us tools that help us confirm that the person sending the message is who we think they are, so we can avoid getting tricked by an impersonator.

# Math for secrets
    
This website focuses on teaching kids the tools that modern cryptography gives us to keep secrets and detect impersonators. These tools are encryption algorithms, hash functions, and digital signatures.  We will also talk about ways to change written messages into mathematical numbers, which we need to do before using any of these tools.  Lastly, we will talk about the threat posed by very powerful computers.  If a computer is powerful enough, it can hack into an encrypted message—unless we use large enough numbers.

### Encryption and Decryption

_Symmetric Encryption:_ Uses the same key for both encryption and decryption. Algorithms like AES (Advanced Encryption Standard) are widely used for encrypting data at rest and in transit.

_Asymmetric Encryption (Public Key Cryptography):_ Uses a pair of keys—public and private keys. The public key is used for encryption, and the private key is used for decryption. Algorithms like RSA and elliptic curve cryptography (ECC) are fundamental for secure communication over the internet.

### Hash Functions

Imagine you have a magical box. Whatever you put inside the box, it gives you back a unique sticker that represents exactly what's inside. If you put the same thing in the box again, you get the same sticker. But if you change even a tiny bit of what's inside, the sticker you get is completely different.

In computers, hash functions are like that magical box. They take any message (or data) and turn it into a short string of numbers and letters, called a hash. If the message changes even a little bit, the hash changes a lot. This is really useful for checking if messages or files have been altered because the same data always gives the same hash.

Hash functions process data to produce a fixed-size string of bytes (a hash). They are designed to be one-way functions, making it infeasible to reverse the hash back to the original data. Hash functions like SHA-256 are crucial for integrity verification, password storage, and blockchain technology.

### Digital Signatures

Let's say you're sending a letter to your friend, but you want to make sure they know it's really from you and not someone pretending to be you. So, you draw a special doodle that only you can draw at the bottom of your letter. When your friend sees that doodle, they know the letter is really from you.

Digital signatures work kind of like that doodle. When you send a message or a document over the internet, you can attach a digital signature. This signature proves that the message or document really came from you, and it hasn't been changed by anyone else after you sent it.

Digital signatures use asymmetric cryptography to simulate the security properties of a handwritten signature on digital documents. They provide proof of origin, identity, and integrity of electronic data. Algorithms like RSA, DSA (Digital Signature Algorithm), and ECDSA (Elliptic Curve Digital Signature Algorithm) are widely used.
