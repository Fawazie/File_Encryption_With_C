# File Encryption With C
This is a C program that encrypts files using an XOR-based cipher. A user-provided key generates a bitmask by summing its ASCII values. Each input character is then XORed with the generated bitmask for encryption. The program reads from a standard input, encrypts the data, and then outputs the data.

## How to Use:

**Tech used:** C.

Download the source.c code provided in the repository.

The encryption and decryption tools can be compiled with. 
```
gcc encrypt.c -o encrypt
gcc decrypt.c -o decrypt

```
Create the file that will be encrypted. This can be a text file or any other format.

Encrypt the file using

```
./encrypt <secret_file>

```
After encrypting the file, you will be given the encrypted file along with the key file.

To decrypt the file, use the code below. 

```
./decrypt <encrypted_file> <key_file>
```
The dec_secret file can be opened and should have the same data.

You can test the effectiveness of the code by trying to decrypt the file with the wrong key

I've attached all the original message files and encrypted and decrypted files for reference purposes in the repo.





