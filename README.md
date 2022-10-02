#Arch-linux-on-Android, I am not a developer. Just making easy for those like me Coming from research/academic community 

#Who wants to use Linux for their daily basis for data analysis/scientific project etc.

#MywebPage: https://sites.google.com/view/achintyabera/tweaks

#setting up gmail or outlook on Arch linux installed using Proot container 

#Systems tested on : Proot, Arch linux, Termux

#Learn from this link https://github.com/LukeSmithxyz/mutt-wizard

#Step by Step commands to follow
1. yay –S mutt-wizard
2. gpg --full-gen-key
3. pass init abc@gmail.com

#Now get a app-based password from gmail/outlook account for which 2FA enabled. Those passwords will be needed for the below command to add account for the mutt-wizard.

3. mw -a abc@gmail.com 

#for sending email put in fish/bash config file

 export EDITOR=nvim

#Change to .mbsync file, Remove "[Gmail]All email" from Patterns section, Just keep 

Patterns "INBOX"

#After that, the size of the downloaded gmail will be 1/3 of actual gmail space

5. mbsync -V abc@gmail.com
6. neomutt

#Similar steps for outlook.com email from Microsoft like abc@outlook.com

1. gpg --full-gen-key
2. pass init abc@outlook.com
3. mw -a abc@outlook.com 
4. mbsync -V abc@outlook.com
5. neomutt

#for Switching account press "i1" or "i2" or "i3" depending on the number of emails you have on mutt-wizard
#To get Update from email page, press small letter "o" and to come back to email page again press "Ctrl+c" on terminal
