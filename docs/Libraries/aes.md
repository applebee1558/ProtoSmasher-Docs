# AES

## Generate IV
```lua
string AES.GenerateIV(<none>)
```
Returns a randomly generated 16 character string that can be used as an IV for encryption.

## Encrypt
```lua
string AES.Encrypt(string Secret, string Key, string IV = "n@*fjakAnf983jF")
```
Returns the secret "message" encrypted via AES-128, AES-192, and AES-256. AES mode is dependent on key length. Key length of 16 will use AES-128, length of 24 will use AES-192, and length of 32 will use AES-256. Only those key lengths are accepted.

## Decrypt
```lua
string AES.Decrypt(string Secret, string Key, string IV = "n@*fjakAnf983jF")
```
Returns the encrypted secret in a decrypted form. Follows the same rules as encrypt (see above).