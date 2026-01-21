# EL-cybersecurity-task4

Cyber Security Internship — Task 4 Deliverable
Password Security & Authentication Analysis
Prepared by: Jitta Sharanya
Date: 2026-01-21

1. Password Storage Basics
• Hashing: One-way irreversible transformation of a password.
• Encryption: Reversible transformation of data using keys.
• Common hash types: MD5, SHA-1, SHA-256, bcrypt.

2. Attacking Weak Passwords
• Dictionary attack: Tries passwords from a predefined list.
• Brute force: Tries every possible combination.
• Weak passwords fail due to predictability and low entropy.

3. Tools Used
• Hashcat: GPU-accelerated password cracking tool.
• John the Ripper: Efficient CPU-based cracking tool.
• Online Hash Identifiers: Detects hash format.

4. Authentication Improvements
• Enable MFA for added security.
• Use strong passwords: 12+ chars, mix of symbols, no dictionary words.
• Avoid reuse across sites.

Objective
Understanding what makes a password strong and testing various passwords against password strength tools to identify best practices for creating secure passwords.

Methodology
Test Passwords Created
I created 8 different passwords with varying complexity levels to test different aspects of password security:

Simple Password: password123
Moderate Password: MyPassword2024
Complex Password: Tr0ub4dor&3
Very Complex Password: K9#mX$7nQ2@pL8!
Long Simple Password: thisisaverylongpasswordwithoutcomplexity
Passphrase: Coffee#Morning$Sunrise2024!
Weak Pattern: abcd1234
Strong Balanced: BlueSky42@Night!
Password Strength Analysis Results
1. Simple Password: password123
Estimated Strength: Very Weak (10-20% score)
Crack Time: Seconds to minutes
Issues:
Common dictionary word
Predictable number sequence
No uppercase letters
No special characters
Too short
2. Moderate Password: MyPassword2024
Estimated Strength: Weak to Moderate (30-40% score)
Crack Time: Hours to days
Issues:
Contains dictionary words
Predictable year pattern
Missing special characters
Strengths:
Mixed case letters
Reasonable length
3. Complex Password: Tr0ub4dor&3
Estimated Strength: Strong (70-80% score)
Crack Time: Years
Strengths:
Character substitution (0 for o, 4 for a)
Special characters
Mixed case
Good length
Considerations:
Difficult to remember without password manager
5. Long Simple Password: thisisaverylongpasswordwithoutcomplexity
Estimated Strength: Moderate (50-60% score)
Crack Time: Months to years
Analysis:
Length provides some security
Lack of complexity is a weakness
Vulnerable to dictionary attacks
Easy to remember but not optimal
6. Passphrase: Coffee#Morning$Sunrise2024!
Estimated Strength: Very Strong (80-90% score)
Crack Time: Decades to centuries
Strengths:
Long length
Memorable structure
Mixed character types
Good entropy despite being readable
7. Weak Pattern: abcd1234
Estimated Strength: Very Weak (5-15% score)
Crack Time: Instant to seconds
Issues:
Sequential patterns
Common keyboard sequence
No complexity
Very short
8. Strong Balanced: BlueSky42@Night!
Estimated Strength: Strong (75-85% score)
Crack Time: Years to decades
Strengths:
Good length
Mixed case
Numbers and symbols
Memorable yet secure
Key Findings and Best Practices
What Makes a Password Strong?
Length: Passwords should be at least 12-16 characters long
Complexity: Include uppercase, lowercase, numbers, and special characters
Unpredictability: Avoid dictionary words, personal information, and common patterns
Uniqueness: Each account should have a different password
Randomness: Higher entropy increases security significantly
Password Security Factors by Importance
Length - Most critical factor; each additional character exponentially increases crack time
Character Variety - Using all character types (upper, lower, numbers, symbols)
Unpredictability - Avoiding patterns, dictionary words, and personal information
Uniqueness - Not reusing passwords across multiple accounts
Common Password Attacks
1. Brute Force Attacks
Method: Systematically trying every possible password combination
Defense: Longer passwords with high complexity make brute force impractical
Impact: Simple passwords can be cracked in seconds; complex ones take centuries
2. Dictionary Attacks
Method: Using lists of common passwords and dictionary words
Defense: Avoid common words, phrases, and predictable patterns
Impact: Can crack weak passwords in minutes to hours
3. Hybrid Attacks
Method: Combining dictionary words with numbers/symbols
Defense: Use truly random combinations or strong passphrases
Example: Attacking "password123" by trying "password" + common number patterns
4. Rainbow Table Attacks
Method: Using precomputed hash tables for common passwords
Defense: Use unique, complex passwords and proper password hashing (with salt)
How Password Complexity Affects Security
Mathematical Impact
8-character password: 26^8 ≈ 208 billion combinations (lowercase only)
8-character complex: 94^8 ≈ 6 quadrillion combinations (all character types)
16-character complex: 94^16 ≈ 4.8 × 10^31 combinations
Crack Time Analysis
Simple 8-char: Minutes to hours
Complex 8-char: Years
Complex 12-char: Centuries
Complex 16-char: Beyond current computing capabilities
Advanced Security Considerations
Multi-Factor Authentication (MFA)
Purpose: Adds additional security layers beyond passwords
Types: SMS, authenticator apps, hardware tokens, biometrics
Importance: Even if password is compromised, account remains protected
Password Managers
Benefits:
Generate strong, unique passwords
Store passwords securely
Auto-fill credentials
Sync across devices
Recommended: Use reputable password managers for all accounts
Passphrases
Concept: Long, memorable phrases with modifications
Example: "Coffee#Morning$Sunrise2024!"
Advantages: Easier to remember than random strings while maintaining security
Common Password Creation Mistakes
Using Personal Information: Names, birthdays, addresses
Dictionary Words: Even with number substitutions
Keyboard Patterns: "qwerty123", "asdf1234"
Short Passwords: Less than 12 characters
Password Reuse: Same password across multiple accounts
Predictable Modifications: Adding year or "1" to old passwords
Visible Password Storage: Writing passwords on sticky notes
Not Using Available Character Types: Ignoring symbols or numbers
Recommendations
For Organizations
Implement password policies requiring minimum length and complexity
Enforce multi-factor authentication
Provide password manager licenses
Regular security awareness training
Monitor for compromised passwords
For Individuals
Use unique passwords for each account
Enable MFA wherever possible
Use a reputable password manager
Consider passphrases for memorable accounts
Regularly update passwords for critical accounts
Never share passwords or store them insecurely
Conclusion
Password strength is primarily determined by length and complexity, with length being the most critical factor. While simple passwords can be cracked in seconds, properly constructed complex passwords can take centuries to break with current technology.

The key to good password security is balancing strength with usability - using password managers for maximum security while employing memorable passphrases for critical accounts that might need manual entry. Combined with multi-factor authentication, strong passwords form the foundation of good cybersecurity practices.

The testing revealed that even small improvements in password complexity can result in exponential increases in security, making the effort to create strong passwords a highly effective security investment.

