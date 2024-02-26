# Getting started with cryptography

Modern cryptography is used by phones and computers to keep all of our digital information secret, safe and secure.  It's used everywhere, but most people don't know how it works or even what it does.

The funny thing is, the core algorithms underlying modern cryptography are built using  arithmatic and algebraic concepts that most middle-schoolers would be familiar with.  This website aims to teach the basic concepts of modern cryptography with that in mind.  After learning everything presented here, middle-school students should be able to hide and share secret messages using math that they already understand.

# What is Cryptography?
    
Cryptography is the science of encoding and decoding information to keep it secret and secure from unauthorized access. Throughout history, cryptography has played a crucial role in military and diplomatic communications, evolving from simple substitution ciphers used in ancient times to complex algorithms that protect our digital world today. 

The advent of computers and the internet in the 20th century transformed cryptography, leading to the development of modern cryptography. This era introduced computational algorithms that leverage mathematical theories to secure data, enabling everything from secure online transactions to private communications over the internet.

Modern cryptography gives us a set of mathematical tools that people can use to communicate without anyone else knowing what they're saying. Imagine you wrote a note that said, "Let's meet at the park at 4 PM," but you didn't want anyone else to know about it. With modern cryptography, you can scramble your message into something that looks like nonsense to anyone who finds it—unless they know the secret that allows them to decrypt the message.  Modern cryptography also gives us tools that help us confirm that the person sending the message is who we think they are, so we can avoid getting tricked by an impersonator.

# Math for secrets
    
This website focuses on teaching kids the tools that modern cryptography gives us to keep secrets and detect impersonators. These tools are encryption algorithms, hash functions, and digital signatures.  We will also explain ways to change written messages into mathematical numbers, which we need to do before using any of these tools.  Lastly, we will talk about the threat posed by very powerful computers.  If a computer is powerful enough, it can hack into an encrypted message—unless we use large enough numbers.

### Text encoding

In the realm of modern cryptography, transforming text into numbers is a fundamental step that allows us to apply mathematical algorithms to secure our data. This process, known as encoding, turns the letters and symbols we use in everyday communication into a numerical format that computers can easily manipulate. Let's dive into how this fascinating process works, making the world of digital security accessible and efficient.

At the core of this transformation is the concept of character encoding schemes. One of the most basic and widely recognized schemes is the American Standard Code for Information Interchange, or ASCII. ASCII assigns a unique number to each letter, digit, and symbol. For example, in ASCII, the letter 'A' is represented by the number 65, 'B' by 66, and so on. This allows a computer to represent text as a series of numbers, making it possible to perform cryptographic operations on it.

Once text is encoded into numbers, cryptographic algorithms can take over. These algorithms use mathematical operations to transform these numbers into a scrambled, unrecognizable format, effectively encrypting the message. The beauty of encoding text into numbers lies in the universality of mathematics; it doesn't matter what the original language or symbols were, as they all become numbers subject to the same cryptographic principles.

### Encryption and Decryption

If you wanted to share a secret message with a friend, how could you keep that message secure?  One thing that you could do is put the message in a box that only you and your friend can open.  Other people who don't have a key to the box would not be able to read your messages.

Encryption is like having a box that only opens with a special key.  You use a secret code to scramble the message so only someone with the key can unscramble it.  When we unscramble the note to turn it back into something you can read, that is called decryption.

Modern cryptography gives us two types of encryption: symmetric and asymmetric. Symmetric cryptography is when you and your friend use the same key to lock and unlock the box. You both need to secretly share this one key to read the messages. Asymmetric cryptography, however, is like having a box where anyone can drop a message inside using a public key (like a slot on the box), but only you can open it with your private key. This means you never have to share your special opening key, making it a safer way to get messages from anyone without giving away how to open the box.

_Symmetric Encryption:_ Uses the same key for both encryption and decryption. Algorithms like AES (Advanced Encryption Standard) are widely used for encrypting data at rest and in transit.

_Asymmetric Encryption (Public Key Cryptography):_ Uses a pair of keys—public and private keys. The public key is used for encryption, and the private key is used for decryption. Algorithms like RSA and elliptic curve cryptography (ECC) are fundamental for secure communication over the internet.

### Hash Functions

Imagine you have a magic gadget that turns anything you touch into a unique fingerprint. Every toy, book, or candy gets its own special mark, just like people's fingerprints—no two are the same. If you change something about the item, like putting on a sticker, the gadget gives it a brand new fingerprint. This is similar to how hash functions work in computers. They take any piece of information and turn it into a unique code, or "fingerprint," just for that info.

If someone tries to mess with your stuff, you can use the gadget to check if the fingerprints before and after match. If they do, all is good; if not, you know something's changed. In the digital world, hash functions do the same thing. They help make sure information hasn't been altered. If the unique code stays the same, the data is safe. But if the code changes, it's a sign something might be wrong. Hash functions act like digital detectives, ensuring everything is as it should be.

Hash functions process data to produce a fixed-size string of bytes (a hash). They are designed to be one-way functions, making it infeasible to reverse the hash back to the original data. Hash functions like SHA-256 are crucial for integrity verification, password storage, and blockchain technology.

### Digital Signatures

Let's say you're sending a letter to your friend, but you want to make sure they know it's really from you and not someone pretending to be you. So, you draw a special doodle that only you can draw at the bottom of your letter. When your friend sees that doodle, they know the letter is really from you.

Digital signatures work kind of like that doodle. When you send a message or a document over the internet, you can attach a digital signature. This signature proves that the message or document really came from you, and it hasn't been changed by anyone else after you sent it.

Digital signatures use asymmetric cryptography to simulate the security properties of a handwritten signature on digital documents. They provide proof of origin, identity, and integrity of electronic data. Algorithms like RSA, DSA (Digital Signature Algorithm), and ECDSA (Elliptic Curve Digital Signature Algorithm) are widely used.
