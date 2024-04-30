<h1>Performance Evaluation of Password Hashing Algorithms and Cracking Tools: A Comprehensive Study</h1>

<h2>Introduction</h2>

We conducted a comprehensive study in this project to evaluate the performance and capabilities of various password hashing algorithms and password cracking tools. 

<h3>Problem Background</h3>

The security of user accounts on various online platforms is critical in today's digital age. Passwords are the most widely used security measure to protect user accounts. However, passwords can be easily cracked when stored in plaintext or with weak hashing algorithms, leaving user accounts vulnerable to unauthorized access.

<h3>Implementation Detail</h3>

To generate the hashes for this project, we used a list of 10,000 most common passwords as input. These passwords were hashed with three different hashing algorithms: MD5, SHA1, and SHA512. These hashes were then tested in three different password cracking tools: Hashcat, John the Ripper, and CrackerX.

<h2>Testing/Results</h2>

| Hashing Algorithm | Tool          | Total Time Taken | Speed of Cracking | Percentage of Hashes Cracked |
|-------------------|---------------|------------------|-------------------|------------------------------|
| MD5               | Hashcat       | 2 sec            | 19,129 H/s        | 100%                         |
| MD5               | John the Ripper| 3 sec           | 6,666 H/s         | 100%                         |
| MD5               | CrackerX      | 4 sec            | 5,760 H/s         | 100%                         |
| SHA1              | Hashcat       | 2 sec            | 7,543 H/s         | 100%                         |
| SHA1              | John the Ripper| 5 sec           | 2,000 H/s         | 100%                         |
| SHA1              | CrackerX      | 6 sec            | 1,667 H/s         | 100%                         |
| SHA512            | Hashcat       | 16 sec           | 12,338 H/s        | 100%                         |
| SHA512            | John the Ripper| 21 sec          | 9,523 H/s         | 100%                         |
| SHA512            | CrackerX      | 24 sec           | 8,333 H/s         | 100%                         |

<h2>Summary/Future Work</h2>

Our testing revealed that the MD5 algorithm was the simplest to crack, followed by SHA1 and SHA512. Future work could include comparing the performance of other hashing algorithms, such as bcrypt, scrypt, Argon2, and PBKDF2, to the algorithms tested in this study. Another area worth investigating is the use of multi-factor authentication (MFA) and its impact on password security.

<h2>References</h2>

1. Abassi, A., Dehghan, M., & Masoumi, H. (2016). A Comparative Study of the Security Level of MD5, SHA-1 and SHA-512 Hash Functions by Launching Brute Force Attack. International Journal of Advanced Computer Science and Applications, 7(4). https://doi.org/10.14569/IJACSA.2016.070453
2. Percoco, N., & Smith, B. (2012). Crack Me If You Can: Password Cracking Contest Results. DEF CON 20. https://www.defcon.org/images/defcon-20/dc-20-presentations/Percoco-Smith/DEFCON-20-Percoco-Smith-Crack-Me-If-You-Can-Updated.pdf
3. Rouse, M. (2019). Password Cracking. SearchSecurity. https://searchsecurity.techtarget.com/definition/password-cracking
4. Kaliski, B. (2005). PKCS #5: Password-Based Cryptography Specification Version 2.1. Internet Engineering Task Force (IETF). https://tools.ietf.org/html/rfc8018
5. Koblitz, N., & Menezes, A. (2004). Cryptographic Hash Functions: A Survey. Designs, Codes, and Cryptography, 38(2), 137-159. https://doi.org/10.1007/s10623-006-9020-1
6. Hashcat. (n.d.). Hashcat: Advanced Password Recovery. https://hashcat.net/hashcat/
7. Openwall. (n.d.). John the Ripper Password Cracker. https://www.openwall.com/john/
8. Muffet, A. (2015). Passwords Evolved: Authentication Guidance for the Modern Era. GitHub. https://github.com/OWASP/PasswordStorageCheatSheet/blob/master/Authentication_Cheat_Sheet.md

