Why GhostShare's Source Code (SC) Cannot Be Published

Anonymity Protection:
GhostShare is based on the principle that the sender remains completely anonymous. If the SC were published, someone could analyze the key generation or internal mechanisms and attempt to link a message to its author, which would completely break the OPSEC.

Key Security:
The SC contains the functions that create and manage the AES-256 encryption keys. Publishing these functions would allow an attacker to understand how a key is generated and, in some cases, exploit this to decrypt messages without authorization.

Prevention of Misuse:
GhostShare is designed for ethical and private use. Publishing the SC could allow malicious actors to modify the application to create phishing tools, fraud, or other illegal activities.

Why does my antivirus flag it as a virus? (False positive)

It is common for antivirus software (like Windows Defender) to flag applications compiled from Python (.py) into an executable (.exe) as a potential threat. This is called a false positive. This happens for two main reasons:

The .exe packaging: Tools like PyInstaller package the Python interpreter and your code into a single .exe file. This is a technique also often used by malware to bundle malicious scripts, making antivirus programs suspicious of all applications packaged this way.

Lack of a digital signature: Signed software has a certificate from a trusted authority that proves the publisher's identity and that the code hasn't been tampered with. GhostShare is a free tool and does not have an expensive code-signing certificate. Without this signature, antivirus software trusts it less and is more likely to flag it.

The software is 100% safe. You can verify its security by decompiling the .exe file yourself to analyze its functions, without needing to see the original source code.

What GhostShare Is Used For

Sending completely anonymous messages: The sender is never identified, and no server is used to relay or store the message.

Secure local encryption: Each message is encrypted with AES-256-CBC before being saved in an HTML file. The key is securely transmitted to the recipient and is not stored anywhere.

File sharing: GhostShare allows files to be added as attachments; they are encrypted and can only be accessed after decryption with the correct key.

How to Use GhostShare

Write a message: Launch the application, enter the text to share, and optionally a pseudonym.

Add a file (optional): Attach a file if necessary. The download button only appears if a file is attached, maintaining clean OPSEC by not revealing the feature unless it's used.

Generate the HTML file: The application encrypts the message and any attached file, then creates an HTML file containing the encrypted message.

Send the key to the recipient: Copy the randomly generated key to the clipboard and transmit it via a secure channel (outside of GhostShare).

Recipient decrypts: The recipient opens the HTML file in a browser, pastes the key, and decrypts the message and any attached files.

Strengths of GhostShare & Security Guarantees

100% local: No servers, no databases, no traces. Everything happens on your machine.

Unbreakable Encryption (AES-256-CBC): GhostShare uses one of the most robust encryption algorithms available, trusted by security experts worldwide.

Complete Anonymity: Even if the key is leaked, no one can know who created or transmitted the message. The key is fully encrypted and encoded within the HTML; it is absolutely not stored in plain text and cannot be decrypted without the passphrase.

Transparent Security: The application's integrity can be verified by decompiling the .exe, allowing technical users to confirm there are no backdoors or data leaks.

No updates necessary: Everything works locally, eliminating the risk of a compromised server or forced update. GhostShare is designed as one of the most robust and secure tools to use for private, off-grid communication.

My contacts:

Discord: idkbbywdym

TikTok: @idkbbywdym
