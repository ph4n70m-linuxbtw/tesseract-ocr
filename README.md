![Tesseract OCR is now maintained by Google](https://github.com/ph4n70m-linuxbtw/ocr-with-tesseract/blob/ee5fd8a3f937e14d24a9bd63ff33233cd382ccb0/googletesseract-ocr.jpg)

# ocr-with-tesseract
This is just a small program I made for Linux that uses the BASH shell scripting language that lets you screen grab text and instantly copies it to your clipboard.

It uses three open source programs : flameshot, tesseract-ocr and xclip.
<br>
<br>
<br>
You must first install the required tools to use the program.

Simply run : 

```
sudo apt update && sudo apt install flameshot tesseract-ocr xclip
```

This will update your computer and install the required packages.
<br>
<br>
<br>
You can download the file here : [ocr.sh](https://github.com/user-attachments/files/24364209/ocr.sh)

You can also clone the git repository if you want, but it is not required at all.

If you do need to clone it, run : 

```
sudo apt install git
```

to install git, and then to clone the repo, run : 

```
git clone https://github.com/ph4n70m-linuxbtw/ocr-with-tesseract.git
```
<br>
<br>
<br>
The main file is a .sh BASH file that only includes a very basic command but the file makes it easier to run quickly.

To use it, you first need to go into the directory that the file is in and run : 

```
chmod +x ocr.sh
```

This essentially makes the file executable so that it can easily be used by typing in : 

```
./ocr.sh
```

You can assign this command to a keyboard shortcut, which makes it very fast to copy large bits of text from your screen.
(It is actually what I have done in the Keyboard program on Xubuntu which comes with XFCE)  
<br>
<br>
<br>
What this file is doing : 

It runs the command 'flameshot gui -r | tesseract stdin stdout | xclip -selection clipboard'.

'flameshot gui -r' takes a screenshot from which you can chose the area that you want to screen grab, 
and it pipes the output (screenshot) to tesseract, which takes the screenshot and turns it into text, 
and finally, pipes the text to xclip, which copies the text to your clipboard.

I hope that this project will be useful to you.
<br>
<br>
<br>
You are free to distribute or modify this file whatsoever.
<br>
<br>
Please consider starring this project so that others will see it too :)
