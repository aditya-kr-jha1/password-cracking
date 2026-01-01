Password Cracking (Educational Project)

Overview
This repository is an educational project created to understand how password hashing and cracking work using Hashcat.
It demonstrates dictionary-based attacks on sample password hashes in a legal and ethical learning environment.

This project is strictly for educational purposes only.
Do NOT use these techniques on real systems or passwords without explicit permission.

Objectives
Understand what password hashes are
Learn how dictionary attacks work
Use Hashcat to crack self-generated sample hashes
Practice basic cybersecurity concepts responsibly

Tools Used
Hashcat (Password recovery tool)
Windows PowerShell / Command Prompt
MD5 hash algorithm (for demonstration)

 Repository Structure
password-cracking/
│
├── README.md          → Project documentation
├── hash.txt           → Contains sample password hash
├── wordlist.txt       → Dictionary used for cracking
├── password.txt       → Dummy passwords (for learning only)


 Note:
All passwords and hashes in this repository are dummy and self-created, not real user data.

 How It Works
1️. Generate a Hash (Example)

Example password:
india123

Its MD5 hash:

8d763385e0476c5f29c6b4e45d2d8f8d
Stored in hash.txt


2️. Prepare Wordlist

wordlist.txt contains possible password guesses, for example:

india
india123
password
admin
123456


3️. Run Hashcat Command
hashcat -m 0 -a 0 hash.txt wordlist.txt


Where:

-m 0 → MD5 hash mode

-a 0 → Dictionary attack


4️. Show Cracked Password
hashcat -m 0 --show hash.txt

 Learning Outcomes
Difference between plain text passwords and hashed passwords
Why weak passwords are dangerous
Importance of strong password policies
Ethical use of cybersecurity tools
Ethical Disclaimer
This repository is intended only for learning and academic purposes.

❌ Do NOT:
Crack real user passwords
Attack live systems
Use this knowledge for illegal activities
Always practice ethical hacking with permission.

 Author

Aditya Kumar Jha
Cybersecurity & Computer Science Learner
India
