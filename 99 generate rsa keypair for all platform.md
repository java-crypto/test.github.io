index.md
https://stackedit.io/app#

Cross-platform cryptography
===============
Security warning :warning:
---------------

:warning:This is a **serious warning** regarding the security of the programs shown in these article series.:warning:

Always keep in mind my disclaimer regarding my programs:

### All programs are for educational purposes and are not intended to use in production or any other programs where a  secure solution is needed. ###

### The programs do not have proper exceptional/error handling and in some cases they use unsecure key lengths or other methods that are unsecure. ###

### Never ever use the programs in real life without they are checked by a qualified cryptographic professional. ###

When a program compiles or run it does <u>not</u> mean that it is secure to run it, especially when you just "copy & paste" the solution
into your own software.

I'm trying to avoid typical errors (e.g. converting strings into a byte array without usage of encoding) but sometimes e.g. I'm using the string
representation of a key to get it "cross the platform". The usage of a string in a cryptographic environment is highly dangerous and can lead
to a complete **useless** encryption.

Try it here:

<iframe src="https://paiza.io/projects/e/SU76a3VYIZKZHBO-PdNnyQ?theme=twilight" width="100%" height="500" scrolling="no" seamless="seamless"></iframe>

So why are strings so dangerous? That's easy to answer - in a lot of programming languages strings are <u>immutable</u>. Let's see an example in Java:

```Java
string password = "secretPassword";
... use the password
encryptString(password, "string to encrypt");
// delete string
password = "";
```

Everything looks fine but.. the variable keeping the password was <u>not</u> deleted but is just pointing to a place with an empty string. The former value "secretPassword"
is still available in the device memory (called the heap) and can get found by a memory scanner that is just waiting for grabbing and sending to its owner.

The solutions to this problem is to use only a char or byte array because they can get deleted.

Happy crypting !


