Cryptography
===============

Header style2
---------------

### Hello World, my first github Page ###

*This text will be italic*

**This text will be bold**

This text <u>will</u> be <ins>underlined</ins>, this not.


| Solution | Link | Java | PHP | C# |
| ------ | ------ | :----: | :---: | :--: |
| AES CBC 256 String Encryption | [http://javacrypto.bplaced.net](http://javacrypto.bplaced.net/) | X | X | X |
| RSA 2048 Signature | [http://java-crypto.bplaced.net] | X | X | X |
| RSA 2048 Encryption | [Encryption](http://javacrypto.bplaced.net/) | X |  | X |
| TestAes | [Encryption html](TestAes/index.md) |  | X |  |
| index2.md | [Test](index2.md) |  | X |  |

This site was built using [GitHub Pages](https://pages.github.com/).

AES CBC 256 String encryption: [http://javacrypto.bplaced.net](https://google.com/)

RSA 2048 Signature: [http://java-crypto.bplaced.net](https://pages.github.com/)

RSA 2048 Encryption: [Encryption](http://javacrypto.bplaced.net/)

The website is published under: Your site is published at [https://java-crypto.github.io/test.github.io/](https://java-crypto.github.io/test.github.io/)

---
#### Some blockquotes ####
> nr 1

> nr 2 and last

> nr 3

---

This is the code in Java:
```JAVA
private static byte[] generateRandomKey() {
    SecureRandom secureRandom = new SecureRandom();
    byte[] key = new byte[32];
    secureRandom.nextBytes(key);
    return  key;
}
```

This is the code in PHP:

```PHP
function generateRandomKey()
{
    return openssl_random_pseudo_bytes(32, $crypto_strong);
}
```

This is the code in C#:

```C#
static byte[] generateRandomKey() {
    RNGCryptoServiceProvider rngCsp = new RNGCryptoServiceProvider();
    byte[] key = new byte[32];
    rngCsp.GetBytes(key);
    return key;
}
```

```python
s = "Python syntax highlighting"
print s
```

The keygen is started with

'Keygen keygen = new Keygen();'

Another way ist to end :-)

More information in German is available in http://javacrypto.bplaced.net. Have fun !
