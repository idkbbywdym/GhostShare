Why GhostShare's Source Code (SC) Cannot Be Published

Anonymity Protection:
GhostShare is based on the principle that the sender remains completely anonymous. If the SC were published, someone could analyze the key generation or internal mechanisms and attempt to link a message to its author, which would completely break the OPSEC.

Key Security:
The SC contains the functions that create and manage the AES-256 encryption keys. Publishing these functions would allow an attacker to understand how a key is generated and, in some cases, exploit this to decrypt messages without authorization.

Prevention of Misuse:
GhostShare is designed for ethical and private use. Publishing the SC could allow malicious actors to modify the application to create phishing tools, fraud, or other illegal activities.

What GhostShare Is Used For

Sending completely anonymous messages: The sender is never identified, and no server is used to relay or store the message.

Secure local encryption: Each message is encrypted with AES-256-CBC before being saved in an HTML file. The key is securely transmitted to the recipient and is not stored anywhere.

File sharing: GhostShare allows files to be added as attachments; they are encrypted and can only be accessed after decryption with the correct key.

How to Use GhostShare

Write a message: Launch the application, enter the text to share, and optionally a pseudonym.

Add a file (optional): Attach a file if necessary. If no file is added, the download button remains hidden to reinforce OPSEC.

Generate the HTML file: The application encrypts the message and any attached file, then creates an HTML file containing the encrypted message.

Send the key to the recipient: Copy the randomly generated key to the clipboard and transmit it via a secure channel (outside of GhostShare).

Recipient decrypts: The recipient opens the HTML file in a browser, pastes the key, and decrypts the message and any attached files.

Strengths of GhostShare

100% local: No servers, no databases, no traces.

AES-256-CBC: Extremely robust encryption.

Complete anonymity: Even if the key is leaked, no one can know who created or transmitted it.

No updates necessary: Everything works locally, eliminating the risk of a compromised server.
