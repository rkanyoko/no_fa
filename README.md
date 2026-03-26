A simple draft of what the challenge was testing, 
A test on obtaining password hashes from a database file. This helped a contestant get the admin hash.
One has to crack the has, i prefer using crackstation since it saves on time
Even by the use of normal hashcracking tools like hashcat, it would still work. After all the hash type was simply sha256.

after cracking the hash using crackstation, one gets the password. Use the same admin/"cracked_password" to login to the site. The same site provided when one launches the instant.
After login, one is redirected to the 2FA page,
when one inspects the page, under storage (in a firefox browser) one can see the cookie.
This cookie has the otp code in it.
use decoder.py to get the OTP in plaintext.
