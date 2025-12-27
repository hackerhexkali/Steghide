# Steghide
Steghide is a command-line steganography tool that allows users to securely hide files inside images or audio files and retrieve them later using a passphrase.

Steghide Tutorial

Basic Steps:
```bash
sudo apt update
```
```bash
sudo apt upgrade -Y
```
(This Ensures system has latest security patches and Software version)

Install Steghide:
```bash
sudo apt install steghide -Y
```

After Installation:
```bash
steghide --help
```
(This shows steghide options)

How to Use:
1) Download any image from web or consider using an image in local system
2) Then create a text file: Type in secret message
3) Make sure both the above things are kept in same folder
4) Open the Terminal from that folder
5) To embed the message to image:
```bash
steghide embed --embedfile [eg: text.txt] --coverfile [eg: cover.jpg]
```
6) passphrase would be prompted: type in password (!!Remember the password!!)
7) To extract the message from the image:
```bash
steghide extract --stegofile [eg: cover.jpg]
```
8) passphrase would be prompted: type in password
9) Extraction complete 
