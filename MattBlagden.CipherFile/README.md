# Cipher File

Commandline utility to encrypt, decrypt, and verify files. The tool has several features that make it suitable for long-term use, making files recoverable without requiring storage of key files or even this tool.

* Keys are generated from user-defined passwords.
* Neither keys nor passwords are ever stored.
* A password signature is displayed so the user can verify that the password has been entered correctly on each use.
* Every file is encrypted with a unique key.
* The encrypted-file format includes plaintext labels describing each section, so the file can be understood by a human (programmer), even if this tool is lost.

## Use

cipherfile encrypt *path*
* Encrypts the file(s) at the specified path, with a password entered by the user

cipherfile derypt *path*
* Decrypts the file(s) at the specified path, with a password entered by the user.

cipherfile verifyPassword *path*
* Verifies that the file(s) at the specified path use a common password, entered by the user.

cipherfile verifyIntegrity *path*
* Verifies that the file(s) at the specified path are intact and have not been modified since creation. Does not require a password.
