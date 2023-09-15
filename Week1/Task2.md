# Task 2: Personal Threat Model

## Asset Phone
My phone is the most critical asset I have. If it's compromised and adversary gets full access to it, in short: I'm screwed. As with most people, my phone is sort of a central hub for all of my accounts and services. It contains banking applications, healthcare applications, emails, contacts, social media applications, and so on. Unrestricted access to my phone means unrestricted access to some of the applications.

### Threat & Likelihood
Threat: Adversary gets (full) access to my phone either physically (stealing the device and quessing/cracking/forcing me to give the PIN-code) or remotely (rootkit, remote shell etc.)

The likelihood of adverasy getting remote access to my phone is slim as I trust the phone manufacturer to patch known vulnerabilities in a timely manner. The phone checks for patches automatically multiple times a day and they are applied during idle-hours at night. In theory, using known vulnerabilities, an adversary has at max 24 hours to exploit the vulnerability before my phone automatically applies the patch. The chance of this happening is really slim, in my opinion.

Another option is that I accidentally click on a malicious link that I received in my email and end up getting the phone's "master account" compromised, for example. This way the adversary could technically lock me out of my phone and access whatever data I have backed up in the cloud, possibly even going as far as copying the data on another phone. The likelihood of this happening is from plausible to slim. Once again, I'm trusting the manufacturer that they will detect the new login attempt and prompt my device for two-factor authentication or even lock the account.

The last option that I'll disclose here is that I lose my device physically, accidentally leaving it on public transportation or getting mugged, for example. The likelihood of these happening from all of these scenarios is the highest: me accidentally losing the device being more likely than me being mugged.

### Vulnerability
Weak and easily guessable and repeadet screen-lock/application access code. Although hitting me with a 5$ wrench multiple times enough will make me tell my password eventually... ![Security by XKCD](images/security.png)

### Impact
Assuming adverasry gets full access to my phone (via guessing/forcing me to give access codes), the impact would be critical. I would have to inform multiple services about the incident and create new accounts and passwords. Investigating how much the adversary was able to do would take a long time and some things might go unnoticed. The absolute worst case scenario is that they were
able to access my bank information and clear my accounts and take loans in my name.

### Prevention & Mitigation
To prevent the absolute worst case scenario, I should remove all unnecessary apps from my phone. Such as banking and healthcare apps, social media, and other services I don't need daily or on the go. This would decrease the attack surface and I could access the services from a web browser, if needed. Accessing services via a web browser will require me to authenticate each time instead of being logged in at all times. Enabling multi-factor authentication (password and biometric authentication e.g Apple's Face ID) will help with restricting access to certain applications.

If I lose my phone, I can disable or completely wipe it remotely if I suspect misuse.
