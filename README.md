# Cryptography
## **Sumary**

hash > symmetry > asymmetry (performance)

**Comparing cryptional function link**

## **Hash**
This is a link to understand what are the hash algorithm: [click here](https://medium.com/@thoaikhmt/to%C3%A0n-v%E1%BA%B9n-d%E1%BB%AF-li%E1%BB%87u-v%C3%A0-hmac-5a291adee555#:~:text=Theo%20l%C3%BD%20thuy%E1%BA%BFt%2C%20b%E1%BA%A5t%20c%E1%BB%A9%20h%C3%A0m%20Hash)


# **Demo**
## Asymmetric + Symmetric algorithm
**A { publicKey, privateKey },  B { data, symmetricKey }**
- Can be any symmetricKey

**Step:**
1. A send ***publicKey*** to B
2. B recieves the A's ***publicKey***
3. B encrypt the ***data*** by the ***symmetricKey*** => **encryptData**
4. B encrypt the symmetricKey by the ***A's publicKey*** => **encryptSymmetricKey**
5. B response the data ***{ encryptData, encryptSymmrtrickey }***
6. A get the B's response data
7. A decrypt the ***encryptSymmetricKey***  by A's ***privateKey*** => **symmetricKey**
8. A decrypt the **encryptData** by ***symmetricKey*** => B's **data**

***Note:*** attacker can modify the data??? When you read the data, can it get errors (not found data or read the malicious data)?