Phishing Email Analysis – Task 2

Overview  
This project analyzes a suspicious email sample to identify common phishing indicators. The objective is to understand how attackers spoof email headers, manipulate content, and deceive users using social engineering tactics.

Repository Purpose  
To document the step-by-step analysis of a phishing email, evaluate authentication failures (SPF, DKIM, DMARC), and provide detailed indicators of compromise.

Files Included  
- sample-1161.eml – Raw email file analyzed  
- phishing_analysis.md – Detailed report of the phishing investigation  
- README.md – Summary of the task and key findings

Key Analysis Points  
1. Spoofed Sender Identity  
   The display name "Microsoft account team" is paired with a non-Microsoft email address:  
   `no-reply@access-accsecurity.com`

2. Authentication Failures  
   SPF: none  
   DKIM: none  
   DMARC: permerror  
   These indicate no verification of sender identity, allowing domain spoofing.

3. Suspicious Contact  
   `solutionteamrecognizd03@gmail.com` – A free Gmail account used as a fake support contact.  
   "Recognized" is misspelled as "recognizd".

4. Social Engineering Tactics  
   The message uses fear and urgency, claiming a login from Russia/Moscow, and urges the user to "report the user" quickly.

5. Technical Deception  
   The IP address claimed in the email (103.225.77.255) does not resolve to Russia but to a hosting provider elsewhere, proving geographic spoofing.

6. Language and Grammar Errors  
   Multiple spelling and punctuation issues, which reduce credibility.

Conclusion  
This is a clear phishing attempt designed to impersonate Microsoft and extract user trust or credentials. Proper header analysis, DNS record checking, and awareness of social engineering helped identify and classify the email as malicious.

Recommendation  
Users should avoid interacting with suspicious emails, verify sender domains, and report phishing attempts to internal security teams or email providers.

