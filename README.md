# File Encryption With C
This is a C program that encrypts files using an XOR-based cipher. A user-provided key generates a bitmask by summing its ASCII values. Each input character is then XORed with the generated bitmask for encryption. The program reads from a standard input, encrypts the data, and then outputs the data.

## How to Use:

**Tech used:** C.

Download the source.c code provided in the repository.

Compile the code using. 
```
gcc -o source source.c
```
Create the file that will be encrypted. This can be a text file or any other format.

Run the file using

```
./source my_key < secret.txt > enc_secret.txt
```
The key can be anything, but in my case, it is "my_key"

The file enc_secret.txt can be opened and it will be unreadable data.

To decrypt the file, use the code below. 

```
./source my_key < enc_secret.txt > dec_secret.txt
```
The dec_secret file can be opened and should have the same data.

You can test the effectiveness of the code by trying to decrypt the file with the wrong key using. the code below and opening the file
```
./source wrong_key < enc_secret.txt > dec_secret_wk.txt
```
I've attached all the original message files, as well as encrypted and decrypted files for reference purposes in the repo.


## Optimizations

This project can be optimized by using a secure algorithm like ASE and a hash function like SHA-256 for processing. Libraries like OpenSSL can also be included to enhance security and reduce vulnerabilities



