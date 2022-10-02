#Step by Step commands to follow
1. yay –S mutt-wizard
2. gpg --full-gen-key
3. pass init abc@gmail.com

#Now get a app-based password from gmail/outlook account for which 2FA enabled. Those passwords will be needed for the below command to add account for the mutt-wizard.

3. mw -a abc@gmail.com 

#for sending email put in fish/bash config file
4. export EDITOR=nvim

#Change to .mbsync file, Remove "[Gmail]All email" from Patterns section, Just keep 
5. Patterns "INBOX"

#After that, the size of the downloaded gmail will be 1/3 of actual gmail space

6. mbsync -V abc@gmail.com
7. neomutt

#Similar steps for outlook.com email from Microsoft like abc@outlook.com



 




