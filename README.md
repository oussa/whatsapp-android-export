# Extract WhatsApp DB in 2022, from Android 12 phone, on a Mac

Solution found in this thread: https://forum.xda-developers.com/t/tool-whatsapp-key-db-extractor-crypt6-12-non-root-updated-october-2016.2770982/page-31#post-83629013

Resharing it here as it's so hidden and I only managed to find it after hours of search and multiple attempts and trials (especially that my backup was about 18GB

I managed to de-crypt the WhatsApp database as of today (20.02.2022, so it still works yayy!!)

First:
- enable "usb debugging" in your phone
- verify you have the latest version of java and the android debug bridge drivers in your Mac
- download the .zip https://github.com/p4r4d0x86/WhatsApp-Key-DB-Extractor/archive/v4.7-E1.0.zip
- extract it without changing the overall structure of the folder
- download WhatsApp 2.11.431 (like from android-apk.org) or from http://whatcrypt.com/WhatsApp-2.11.431.apk
- put it in the `tmp` folder replacing (or just renaming it to) `legacywhatsapp.apk`

Second
- launch whatsappkeydbextract.sh file (make sure `chmod +x whatsappkeydbextract.sh` if needed)
- unlock your Android phone when asked and confirm and follow the prompts you get on both the phone and the terminal
- when asked about about a password leave it empty
- the process should finish quite fast (within 1 minute max) and with no errors
- in the end of the process the original WhatsApp app should be restored flawlessly
- check the extracted folder!! you made it :highfive:

Now you can use https://github.com/B16f00t/whapa to play with the exported data including, but not limited to, generating a beautiful report out of your chats
