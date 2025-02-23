# Introduction to RSA Algorithm

- RSA is a public-key cryptographic algorithm, named after the initials of its three developers: Ron Rivest, Adi Shamir, and Leonard Adleman.
- In asymmetric encryption, there are two keys: a public key and a private key. They form a pair. If a message is encrypted with the public key, only the corresponding private key can decrypt it; if encrypted with the private key, only the corresponding public key can decrypt it.
- The process of exchanging confidential information using asymmetric encryption is as follows: Party A generates a pair of keys and publishes one as the public key. Party B, who obtains the public key, uses it to encrypt the confidential information and sends it to Party A. Party A then decrypts the encrypted information using its private key.



# How to use?



## Generate RSA Key



![image-20250223215058224](.HelpDoc.assets/image-20250223215058224.png)



**Generated public and private key log information**

![微信截图_20250223214939](.HelpDoc.assets/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223214939.png)



**Generated encrypted file**



![image-20250223215020613](.HelpDoc.assets/image-20250223215020613.png)







## Load the key file

![image-20250223215427695](.HelpDoc.assets/image-20250223215427695.png)





## Public key encryption + private key decryption



![image-20250223215909672](.HelpDoc.assets/image-20250223215909672.png)







**Print results:**

![image-20250223215848029](.HelpDoc.assets/image-20250223215848029.png)



## Base64 Encode/Decode

These two nodes are to solve the problem of data loss in binary to string conversion



1. **Transmission of Binary Data in Text Protocols**  
   Early communication protocols (such as email) only supported the transmission of ASCII characters and could not directly handle binary data (e.g., images, videos, etc.). Base64 encoding converts binary data into a text format composed solely of ASCII characters, ensuring that the data is not corrupted or lost during transmission.

2. **Compatibility Issues with Special Characters**  
   Certain characters (such as control characters or non-ASCII characters) may be misinterpreted or filtered during transmission, leading to data corruption. Base64 encoding maps binary data to safe printable characters (A-Z, a-z, 0-9, +, /), avoiding this issue.



![image-20250223220504049](.HelpDoc.assets/image-20250223220504049.png)