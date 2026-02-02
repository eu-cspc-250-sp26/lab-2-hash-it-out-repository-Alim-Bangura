# Hash It Out Lab - Submission

**Student Name:** [Your Name Here]  
**Date:** [Submission Date]  
**CSPC 250: Computer Systems Security**

---

## Part 1: Understanding Hashes (10 points)

### Exercise 1.1: Create Your First Hash

**1. What is the MD5 hash of your name?**

a53d8b0dbd48439b5c5e235fa8e78829 
**2. Run the command again with the exact same name. Did the hash change? Why or why not?**

No the hash did not change becasue the input is the same 

**3. Change one letter of your name (like capitalizing it) and run again. How different is the hash?**

The hash is very different there are no similarities at all.

---

### Exercise 1.2: Hash Collisions

**4. What is the md5sum of the file you created?**

a53d8b0dbd48439b5c5e235fa8e78829 

**5. In your own words, explain what a hash collision is and why it's a security concern.**

A hash collsion is when 2 different inputs taht have the same hash output.

---

## Part 2: Password Storage (10 points)

### Exercise 2.1: Examine the Shadow File

**6. Why would a system have users with `*` instead of password hashes?**

This means that there is no password hash that exsits becasue * cannot be hashed, so password login is impossible.

**7. What do the different parts of karl's password line mean? (Hint: Research the format of `/etc/shadow` entries)**

User- karl, $y - yescrypt hashing algorithm, pass change: day 19255 since 1970, expires after 99999 days, warning- 7 days before expiration


---

### Exercise 2.2: Understanding Password Hashing

**8. Why don't systems store passwords in plaintext?**

Systems dont store passwords in plain text becasue it will make user accounts and systems really easy to invade

**9. What is a "salt" in password hashing and why is it used?**

The salt is a random data added to a password before hashing, it is used because it prevents same passwords from having the same hashes.

**10. Research the `yescrypt` algorithm (the `$y$` prefix). Why is it considered secure?**

It is considered secure becasue it causes each password attempt to use large amounts of memory space and slows down cracking softwares and 

---

## Part 3: Password Cracking (15 points)

### Exercise 3.1: Crack Karl's Password

**11. What was karl's password?**

karl:test:19255:0:99999:7:::
**12. How long did it take John to crack it?**

0:00:00:03

**13. Why was this password easy to crack?**

I think that karls password was easy to crack becasue it used his name and didnt have enough randomness in it or speacial characters.

---

### Exercise 3.2: Verify the Password

**14. Does the hash match? (Yes/No)**

Yes

**15. What does this tell you about how Linux verifies passwords during login?**

it checks passwords by comparing hashs instead of real passwords.

---

## Part 4: Security Analysis (5 points)

**16. Based on this lab, what makes a password "strong"?**

A strong pass word should have a minimum of 8 characters with at least one speacialized character and show have an uppercase, these all mean that there should be lots of randomness in your password

**17. Why do websites now require passwords with numbers, symbols, and mixed case?**

To increase the randomness

**18. If you were designing a password policy for a company, what rules would you set? (At least 3 specific rules)**

1. password should be at least 10 characters long
2. password should have a minimum of 2 speacialized characters
3. passwords should have at least 3-4 digits in them

---

## Screenshots Checklist

Include three screenshots in the `screenshots/` folder:

- [ ] `screenshot1.png` - Your name being hashed (Exercise 1.1)
- [ ] `screenshot2.png` - md5sum of your file (Exercise 1.2)
- [ ] `screenshot3.png` - John the Ripper cracking karl's password (Exercise 3.1)

---

## Reflection (Optional but Recommended)

What was the most interesting thing you learned in this lab?

[Your answer here]

---

## Academic Integrity Statement

By submitting this lab, I affirm that:
- I completed this work independently
- I did not copy answers from other students
- I did not use AI tools to generate my responses
- I understand the concepts and can explain them in my own words

**Signature (type your name):** Alim   
**Date:** 2/1/2026
