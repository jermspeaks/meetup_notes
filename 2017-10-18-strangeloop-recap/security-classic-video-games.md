# The Security of Classic Game Consoles 
by Kevin Shekleton

## Info

> It's 1986 and you're sitting a few feet away from your 19" CRT television. Blowing the dust out of your Super Mario cartridge you insert it into your Nintendo and push the power button. The familiar music plays and you’re sucked into a world of goombas and castles on your quest to save Princess Peach. While engrossed in your game, you probably didn't realize the engineering that went into the security of your game and console.

> Join me as we travel back through history and explore the security of classic game consoles. You don't have to be a gamer to appreciate the various security methods that were employed, including hardware, media, and software security measures. Learn how many of these security measures were exploited, either directly or indirectly, as well as the security measures which have yet to be broken.

> You'll leave this fun presentation with not only an understanding of the technical details of what went into protecting the security of your favorite classic game consoles and how they were broken, but also how we can apply these historical lessons learned to the modern software and systems we build today.

> Kevin Shekleton
> [CERNER](https://www.cerner.com/)

> Kevin Shekleton is a VP & distinguished engineer at Cerner, a leading developer of healthcare software. At Cerner, he serves as the technical lead for cybersecurity strategy and implementation, mobile applications, and contemporary healthcare interoperability standards. A true geek at heart, he is passionate about programming, open source, comic books, and of course, classic video games.

## Notes

- Nintendo came into the market at an interesting time
- Video game crash of 1983

- Lots of references back to this [1975 paper](http://web.mit.edu/Saltzer/www/publications/protection/Basic.html)
	- The Protection of Information in Computer Systems
	- Saltzer, J & Schroder M (1975)

### NES

- "This seal is your assurange that Nintendo has approved and guaranteed the quality of this product"
- Friday the 13th one of the worst games to have this seal first.
- 2 years of exclusivity (that's what the seal meant)
- Nintendo constrained the market: only 5 games per developers
- Content review with Nintendo
- Nintendo controlled all manufacturing, upfront payments, no returns

### Playstation

- Parallel Port - inject proper region header into data stream

> Least privilege:
> Every program and every user of the system should *operate using the least set of privileges* necessary to complete the job. Primarily, this principle limits the damage that can result from an accident or error. It also reduces the number of potential interactions among privileged programs to the minimum for correct operation, so that *unintentional, unwanted, or improper uses of privilege are less likely to occur.* Thus, if a question arises related to misuse of a privilege, the number of programs that must be audited is minimized. Put another way, if a mechanism can provide "firewalls," the principle of least privilege provides a rationale for where to install the firewalls. The military security rule of "need-to-know" is an example of this principle.

> Economy of mechanism:
> *Keep the design as simple and small as possible.* This well-known principle applies to any aspect of a system, but it deserves emphasis for protection mechanisms for this reason: design and implementation errors that result in unwanted access paths will not be noticed during normal use (since normal use usually does not include attempts to exercise improper access paths). As a result, techniques such as line-by-line inspection of software and physical examination of hardware that implements protection mechanisms are necessary. For such techniques to be successful, a small and simple design is essential.

- Today, we call this "KISS": Keep it simple, stupid

> The Protection of Information in Computer Systems

- In 1999, Sony removed the parallel port in Playstation

### Dreamcast

- Three formats the Dreamcast can read: CD-ROM, GDROM, MILCD
- GDROM & MILCD are propriatary
- MILCD: Audio track + executable code
- Attackers took the GDROM and copied it to MILCD (down sampled)

- Attacks follow the path of least resistance

### Today

- Work factor of modern console hardware has surpassed effort
- Modding are too risky, circuits too integrated
- Attackers moved from hardware to software

- **Phantasy Star Online** on Nintendo Gamecube
- Connect to a local malicious server via DNS hijacking
- OS is rooted through execution of malicious code that masquerades as an upgrade to the game

- **The Legend of Zelda, Twilight Princess** on Nintendo Wii
- Malicious save game file results in buffer overflow when reading in the name of Link's horse
- OS is rooted through execution of malicious code

- Nintendo Switch
- WebKit vulnerabilities because shipped with older version of WebKit (6 months old)