# PW-Crack-3
Cylab CTF PW Crack 3

Q: Can you crack the password to get the flag? Download the password checker here https://challenge-files.cylabacademy.net/library/2b741086a592ccabd501acc798dfc974c0193e71c166b3addef3f87a6e572943/level3.py
 and you'll need the encrypted flag https://challenge-files.cylabacademy.net/library/2b741086a592ccabd501acc798dfc974c0193e71c166b3addef3f87a6e572943/level3.flag.txt.enc
 and the hash https://challenge-files.cylabacademy.net/library/2b741086a592ccabd501acc798dfc974c0193e71c166b3addef3f87a6e572943/level3.hash.bin
 in the same directory too.

There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

Hint1: To view the level3.hash.bin file in the webshell, do: $ bvi level3.hash.bin

Hint2: To exit bvi type :q and press enter.

Hint3: The str_xor function does not need to be reverse engineered for this challenge.

Step1: Download all the files level3.flag.txt.enc,level3.hash.bin and level3.py
wget https://challenge-files.cylabacademy.net/library/2b741086a592ccabd501acc798dfc974c0193e71c166b3addef3f87a6e572943/level3.py
wget https://challenge-files.cylabacademy.net/library/2b741086a592ccabd501acc798dfc974c0193e71c166b3addef3f87a6e572943/level3.flag.txt.enc
wget https://challenge-files.cylabacademy.net/library/2b741086a592ccabd501acc798dfc974c0193e71c166b3addef3f87a6e572943/level3.hash.bin

Step2: Open file level3.py
cat level3.py
and copy all the password: "8799", "d3ab", "1ea2", "acaf", "2295", "a9de", "6f3d"

Step3: python3 level3.py and try entering password one by one.  a9de is the password.

<img width="538" height="187" alt="image" src="https://github.com/user-attachments/assets/9c3b1f94-a8ea-4fcd-8786-71e6bc95cb6e" />

Step4: Final Answer:academy{m45h_fl1ng1ng_de530414}

