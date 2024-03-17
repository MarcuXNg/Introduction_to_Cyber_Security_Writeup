### Common attacks:

- Log in: use a long list passwords with an automated tool to test them against the login page to discover the password
- Searching: adding specific characters and codes to the search term for the target system to return data it should not or execute a program it should not.
- Provide payment details: The attacker would check if the payment details are sent in cleartext or using weak encryption. Encryption refers to making the data unreadable without knowing the secret key or password.

### Identification and Authentication Failure

Identification refers to the ability to identify a user uniquely
Authentication refers to the ability to prove that the user is whom they claim to be.

Weakness:
- Allowing attackers to use brute force,... try many password (automated tools) to find valid login credentials
- Allowing user choose a weak password (easy to guess)
- Storing users' password in plain text. If the attacker manages to read the file containing the passwords. If the attacker manages to read the file containing the passwords, we don’t want them to be able to learn the stored password.

### Broken Access Control

- Access control ensures that each user can only access files (documents, images, etc.) related to their role or work.
- Vulnerabilities related to access control include:
+ Failing to apply the principle of the least privilege and giving users more access permissions than they need.
+ Being able to view or modify someone else’s account by using its unique identifier.
+ Being able to browse pages that require authentication (logging in) as an unauthenticated user. 

### Injection

- An injection attack refers to a vulnerability in the web application where the user can insert malicious code as part of their input. 
- One cause of this vulnerability is the lack of proper validation and sanitization of the user’s input.

### Cryptographic Failures

- Cryptography focuses on the processes of encryption and decryption of data.
- Encryption scrambles cleartext into ciphertext, which should be gibberish to anyone who does not have the secret key to decrypt it.
- Encryption ensures that no one can read the data without knowing the secret key.
- Decryption converts the ciphertext back into the original cleartext using the secret key.

[Examples]

- Sending sensitive data in clear text, for example, using HTTP instead of HTTPS. HTTP is the protocol used to access the web, while HTTPS is the secure version of HTTP. Others can read everything you send over HTTP, but not HTTPS.
- Relying on a weak cryptographic algorithm. One old cryptographic algorithm is to shift each letter by one.
- Using default or weak keys for cryptographic functions. 