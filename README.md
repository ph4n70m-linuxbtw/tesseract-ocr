# ocr-with-tesseract
This is just a small program I made for Linux that uses the BASH shell scripting language that lets you screen grab text and instantly copies it to your clipboard.

It uses three open source programs : flameshot, tesseract-ocr and xclip.

You must first install the required tools to use the program.

Simply run : 

```
sudo apt update && sudo apt install flameshot tesseract-ocr xclip
```

This will update your computer and install the required packages.

You can download the file here : [ocr.sh](https://github.com/user-attachments/files/24364209/ocr.sh)

It is a .sh BASH file that only includes a very basic command but makes it easier to run quickly.

To use it, you first need to go into the directory that the file is in and run : 

```
chmod +x ocr.sh
```

This essentially makes the file executable so that it can easily be used by typing : 

```
./ocr.sh
```

You can assign this command to a keyboard shortcut, which makes it very fast to copy large bits of text from your screen.
(It is actually what I have done in the Keyboard program on Xubuntu which comes with XFCE)
