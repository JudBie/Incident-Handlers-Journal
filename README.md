# Incident Handler's Journal

## Project Description
This journal documents my hands-on experience investigating and responding to various cybersecurity incidents as part of my security analyst training. Through these entries, I practiced the essential skill of documenting security incidents using the 5 W's framework (Who, What, When, Where, Why) and learned to use various security tools for incident detection and response. This journal serves as both a learning record and a demonstration of my ability to systematically analyze and document security incidents.

## What I Learned
- How to properly document security incidents using the 5 W's framework for comprehensive incident analysis
- The critical importance of maintaining an incident handler's journal for tracking patterns and supporting investigations
- How to use VirusTotal to analyze suspicious files in a sandbox environment and interpret the results
- How to follow security playbooks to make escalation decisions during incident response
- How to identify various attack vectors including phishing, ransomware, forced browsing attacks, and social engineering
- The real-world business impact of different types of security incidents on healthcare, financial services, and retail organizations
- How to recognize indicators of compromise such as grammatical errors in emails, sender/name mismatches, and suspicious file attachments
- The importance of timely incident response and the consequences of dismissing potential threats as spam
- How attackers exploit human psychology through social engineering tactics like fake job applications and password-protected files

## Tools Used
- **VirusTotal** - Online malware scanning and file analysis tool that uses multiple antivirus engines to detect malicious files in a sandbox environment
- **Security Playbooks** - Step-by-step incident response guides with visual flowcharts for decision-making and escalation procedures
- **Incident Handler's Journal** - Documentation framework using the 5 W's to systematically record and analyze security incidents
- **Final Reports** - Comprehensive incident documentation for tracking investigations and outcomes

## Journal Entries

### Entry 1: Ransomware Attack on Healthcare Clinic
![Ransomware Healthcare Attack Part 1](images/entry1-ransomware-part1.png)
![Ransomware Healthcare Attack Part 2](images/entry1-ransomware-part2.png)

**Date**: August 6, 2025

**Incident Type**: Ransomware Attack

**Tools Used**: None

**The 5 W's:**

- **Who**: A group of unethical hackers targeting healthcare and transportation businesses
- **What**: Hackers deployed ransomware through phishing emails. Employees downloaded malicious content, which encrypted all important patient medical files and brought business operations to a halt. A ransom note was left demanding payment for the decryption key.
- **When**: Tuesday morning at 9:00 AM
- **Where**: A small U.S. healthcare clinic
- **Why**: Employees downloaded content from a phishing email, giving hackers access to the company's network. The attackers were financially motivated, demanding ransom payment in exchange for decrypting the files.

**My Analysis**: This incident demonstrated how phishing remains one of the most effective attack vectors. The healthcare sector is particularly vulnerable because patient care depends on immediate access to medical records. When ransomware encrypted these critical files, the clinic had to stop operations entirely, putting patients at risk. The financial motivation was clear from the ransom note. This entry helped me understand the real-world impact of ransomware attacks and why employee security awareness training is crucial.

**Key Question**: What security measures did the clinic already have in place to prevent or detect this type of attack?

---

### Entry 2: Malicious Spreadsheet Investigation with VirusTotal
![Malicious Spreadsheet Entry Part 1](images/entry2-virustotal-part1.png)
![Malicious Spreadsheet Entry Part 2](images/entry2-virustotal-part2.png)

**Date**: August 26, 2025

**Incident Type**: Phishing Email with Malicious Payload

**Tools Used**: VirusTotal - A sandbox environment tool that analyzes files to determine if they are malicious

**The 5 W's:**

- **Who**: A malicious actor who sent a phishing email to an employee
- **What**: An employee received an email containing a password-protected spreadsheet. After downloading and entering the provided password, a malicious payload was activated on the employee's computer.
- **When**: Tuesday, August 26, 2025 at 1:11 PM
- **Where**: At a financial services office
- **Why**: The employee downloaded and opened the malicious spreadsheet using the password provided in the email

**My Analysis**: This was my first time using VirusTotal, and it was challenging but valuable. The password protection on the spreadsheet was a clever social engineering tactic - it added a sense of legitimacy and required the employee to take an active step (entering the password), which helped bypass some security measures. Using VirusTotal's sandbox environment allowed me to safely analyze the file without risking further infection. This incident taught me how attackers use seemingly legitimate business scenarios (like receiving a document) to deploy malware.

**Key Questions**: 
- Did the employee recognize any signs that this might be a phishing email?
- Why was the spreadsheet password protected? (This was likely to evade automated security scans)

---

### Entry 3: Phishing Email Investigation Using Playbook
![Phishing Investigation Playbook Part 1](images/entry3-playbook-part1.png)
![Phishing Investigation Playbook Part 2](images/entry3-playbook-part2.png)

**Date**: August 27, 2025

**Incident Type**: Phishing Email Investigation (Follow-up to Entry 2)

**Tools Used**: Security Playbook - Provided step-by-step guidance with visual flowcharts to determine if the email needed escalation

**The 5 W's:**

- **Who**: A malicious actor who sent an email to an HR employee using the fake name "Clyde West"
- **What**: The attacker sent an email claiming to be interested in an engineering job posting on the company's website. The email included a password-protected spreadsheet supposedly containing their resume, with the password provided in the email.
- **When**: Wednesday, July 20, 2022 at approximately 9:30 AM
- **Where**: HR department at Ingergy offices
- **Why**: The HR employee believed the malicious file was a legitimate resume from "Clyde West" and opened it using the provided password

**My Analysis**: Using the playbook was extremely helpful for structured investigation. It gave me a clear decision-making framework to follow. Through the playbook process, I identified multiple red flags that confirmed this was a legitimate phishing alert:
- **Grammatical errors** in the email body
- **Sender email/name mismatch** - the email address didn't match "Clyde West"
- **Hash value analysis** confirmed the attached file was malicious

The playbook's visual flowchart was particularly useful when I struggled to understand written instructions. This incident taught me the value of following established procedures during incident response and how to identify phishing indicators systematically.

**Key Insight**: This entry demonstrates how attackers exploit HR processes by impersonating job applicants, taking advantage of HR employees' expectation to receive resumes from unknown individuals.

---

### Entry 4: Forced Browsing Attack - Customer PII Theft
![PII Theft Forced Browsing Part 1](images/entry4-pii-theft-part1.png)
![PII Theft Forced Browsing Part 2](images/entry4-pii-theft-part2.png)

**Date**: August 29, 2025

**Incident Type**: Forced Browsing Attack / Data Breach

**Tools Used**: Final Report - Documentation of the complete incident investigation

**The 5 W's:**

- **Who**: A malicious attacker who gained unauthorized access to customer PII (Personally Identifiable Information)
- **What**: The attacker exploited a vulnerability on the company's e-commerce webpage using a forced browsing attack to steal customer PII. On December 22, 2022 at 3:13 PM PT, the attacker sent a ransom email demanding $25,000 to keep the data private. The employee dismissed it as spam. Six days later (December 28, 2022 at 7:20 PM PT), the attacker sent a second email with proof of the stolen data and doubled the ransom to $50,000. The employee then reported it to the security team.
- **When**: The incident was reported on December 28, 2022 at approximately 7:20 PM PT
- **Where**: The attack occurred through the company's e-commerce webpage. The investigation was conducted at the office after an employee reported it to the security team.
- **Why**: A vulnerability in the e-commerce webpage allowed the attacker to perform a forced browsing attack. The attacker manipulated the URL (specifically changing order numbers) to access unauthorized customer information.

**My Analysis**: This incident highlighted the serious consequences of web application vulnerabilities. The forced browsing attack technique involved directly manipulating URLs to access resources that should have been restricted. The escalation from $25,000 to $50,000 when the first email was ignored shows how attackers exploit delays in incident response. The employee's initial dismissal of the first email as spam demonstrates why security awareness training is critical - even legitimate threats can initially appear suspicious. This case taught me about web application security weaknesses and the importance of proper access controls and input validation.

**Key Question**: What security controls were already in place that might have helped detect this incident earlier? (Could have prevented the 6-day delay before the threat was taken seriously)

---

## Reflections and Key Takeaways
![Reflections and Notes](images/reflections-notes.png)

### 1. Were there any specific activities that were challenging for you? Why or why not?

Investigating a file using VirusTotal was challenging for me. I had never used VirusTotal before, so learning what to look for and understanding the information it provided took time. However, this challenge helped me develop practical skills in malware analysis and file investigation that are essential for security work.

### 2. Has your understanding of incident detection and response changed since taking this course?

Yes, significantly. I now understand what incident detection and response truly means and the various tools involved. Before taking this course, I thought incident response was primarily about constantly using security tools. However, I learned that much more is involved - particularly the importance of proper documentation. Maintaining an incident handler's journal is a crucial part of incident detection and response. This documentation creates a knowledge base, tracks patterns, and provides valuable information for future investigations.

### 3. Was there a specific tool or concept that you enjoyed the most? Why?

I enjoyed using VirusTotal the most. Despite initially finding it challenging, I came to appreciate how useful this tool can be. I was able to connect theoretical concepts I was learning with practical, real-world analysis. Seeing how the tool works in a sandbox environment and understanding the detection results helped solidify my understanding of malware analysis and threat detection.

---

## Summary

Through these four documented incidents, I demonstrated the ability to systematically investigate and document various types of cybersecurity threats including ransomware attacks, phishing campaigns, social engineering, and web application vulnerabilities. Each entry showcases different aspects of incident response:

- **Incident Analysis**: Using the 5 W's framework to thoroughly document each incident
- **Tool Proficiency**: Hands-on experience with VirusTotal, security playbooks, and incident documentation
- **Pattern Recognition**: Identifying indicators of compromise and attack techniques
- **Critical Thinking**: Questioning security gaps and analyzing root causes
- **Business Impact Awareness**: Understanding how security incidents affect different industries

This journal represents my growth from initial challenges (learning VirusTotal) to confident application of security tools and frameworks. Most importantly, I learned that effective incident response isn't just about technical tools - it's about systematic documentation, following established procedures, and maintaining detailed records that support both immediate response and long-term security improvements.
