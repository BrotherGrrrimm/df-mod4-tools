# df-mod4-tools
# Required
1. Create github repository df-mod4-tools
2. Clone repository to machine

## Exercise 1: Autopsy - Import Hash Database (of Known files)
I went to sourceforge.net and downloaded latest NSRL file. (this file is 1.7 GB, not the 1.3 GB as mentioned in the instructions)
I imported the hash file to autopsy. Tools > Options > Hash Sets > Import Hash Set
## Exercise 1: Screeenshot
[Mod4ex1ImportedHashFile](https://github.com/user-attachments/assets/05ca47b2-6157-4b4f-9f33-294e2ba708da)

Having a hash database in Autopsy is valuable because it allows an investigator to quickly search for known hashes, and then focus on the ones that do not match.

## Exercise 2: Autopsy - Create Hash Database (of Evidence files)
1. I created a new investigation in autopsy
2. I added the data source and ran the ingest modules.
3. I tagged the evidence files with Key Words "Special Project-A" with a tag of the same name.
4. When I attempted to generate the report, I got an error message. ""Error generating report: java.lang.NoSuchFieldError: Factory" I put this message into Co-Pilot and apparently it is a known error Autopsy is looking into. In the Autopsy Github Issues Community it says they are working on a solution and it will be available soon, but was not availavle as of this assignment. Instead I exported the tagged files to a csv.
5. I created the new Hash Database for Special Project-A and added the four known bad hashes.
## Exercise 2: Screenshot
[Create Hash Database](Mod4ex2CreateHashDatabase.png)

## Exercise 3: Hex Editor - Match File Remnants
1. I created a blank Word document named "evidence1.docx" 
2. I calculated the Hash in PowerShell and in ImHex and verified that the two matched.
## Exercise 3: Screenshot 1
[Calculate & Verify Hash](Mod4CalculateandVerifyHash.png)
## Exercise 3: Screenshot 2
[Hex Editor Match File Remnants](Mod4ex3HexEditormatchFileRemnants.png)
Being able to view the hash files of individual sectors is helpful because you can tell if data has been altered or deleted.

## Exercise 4: Simple Encryption
1. I created a new directory named "ex4" in my repo.
2. I created a new text file called "evidence.txt" and entered some text.
3. I copied the text into cyberchef's input area and located the encryption code. 
4. I encoded the text and saved the encoded text as "nothing.txt"
5. I located the decryption code, entered my key, and decrypted the encrypted message saving it as "recovered.txt"
## Exercise 4: Screenshot
[Simple Encryption](Mod4ex4SimpleEncryption.png)
Bit shifting involves moving binary bits of data to the left or right in their binary representation. Bit shifting can be used to conceal evidence that the foreensic investigator will then need to bring back together to reveal. It is often used in calculations, encoding/decoding, and manipulating flags in data.
