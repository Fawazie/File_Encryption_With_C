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

Optimizing the page to be responsive to fit any device and screen size meant the website would go through various iterations before being able to be as imagined. Using media queries was my initial method of keeping the page responsive but it was clear the method was very tedious and lacked the ability to fit any screen size effortlessly. To combat this issue I was forced to redesign the entire page. During the redesign, I could commit to a design that kept the page responsive by dividing the page into sections relative to each other.

## Lessons Learned:

This was my very first attempt at building a page with HTML, CSS, and Javascript so every single time I worked on the site I learned something new, whether it was something as minute as making the sections relative to each other to allow them to flow into each other and be visually pleasing or something as important like learning how to implement media queries correctly. I was also able to learn things like how a color scheme can vastly improve the looks of a website and with the help of CSS I was able to include small touches that make the page pop like gradients around the projects that implement the color scheme of the language they were built by, an example would be the blue and yellow around the calculator which are also the colors of the python language 


