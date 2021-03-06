---
layout: article
title: What encryption is being used?
categories: [security]
featured: true
popular: false
tags: [encryption]
---

Bitwarden uses [AES][aes]{:target="blank"} 256 bit encryption as well as [PBKDF2][pbkdf2]{:target="blank"} to secure your data.

[AES][aes]{:target="blank"} is used by the US government and other government agencies around the world for protecting top secret data. With proper implementation and a strong encryption key (your master password), AES is considered unbreakable.

[PBKDF2][pbkdf2]{:target="blank"} is used to derive the encryption key from your master password. This key is then salted and hashed.

Bitwarden does not write any crypto code. Bitwarden only invokes crypto from popular and reputable crypto libraries that are written and maintained by cryptography experts. The following crypto libraries are used:

- JavaScript (web, browser extension, desktop, and CLI vaults)
  - [Forge][forge]{:target="blank"}
  - [Web Crypto][webcrypto]{:target="blank"}
  - [Node.js Crypto][nodecrypto]{:target="blank"}
- C# (mobile vault)
  - CommonCrypto (iOS, Apple)
  - Javax.Crypto (Android, Oracle)
  - [BouncyCastle][bouncy]{:target="blank"} (Android)

Bitwarden **always** encrypts and/or hashes your data on your local device before it is ever sent to the cloud servers for syncing. The Bitwarden servers are only used for storing encrypted data. It is not possible to get your unencrypted data from the Bitwarden cloud servers.

[aes]: https://en.wikipedia.org/wiki/Advanced_Encryption_Standard
[pbkdf2]: https://en.wikipedia.org/wiki/PBKDF2
[forge]: https://github.com/digitalbazaar/forge
[webcrypto]: https://w3c.github.io/webcrypto/Overview.html
[bouncy]: http://www.bouncycastle.org/csharp/
[nodecrypto]: https://nodejs.org/api/crypto.html
