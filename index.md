#Cryptography

##Header systele2

Hello World, my first github Page

*This text will be italic*
**This text will be bold**

This the code in Java:
```java
    private static byte[] generateRandomKey() {
        SecureRandom secureRandom = new SecureRandom();
        byte[] key = new byte[32];
        secureRandom.nextBytes(key);
        return  key;
    }
```

This the code in PHP:
```php
function generateRandomKey()
{
    return openssl_random_pseudo_bytes(32, $crypto_strong);
}
```

This the code in C#:
```c#
    static byte[] generateRandomKey() {
        RNGCryptoServiceProvider rngCsp = new RNGCryptoServiceProvider();
        byte[] key = new byte[32];
        rngCsp.GetBytes(key);
        return key;
    }
```

More information in German is available in http://javacrypto.bplaced.net. Have fun !
