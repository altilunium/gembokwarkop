# gembokwarkop
casual encryption for daily use

> vt/112.024.233 (21.5.26 13.54.04) : The plaintext is encoded with Base64, then encoded again with Vigenere cipher.
>
> vt/112.025.261 (21.5.26 15.31.23) : I know, right? Tried to brute force them through DeepSeek and Claude, and the former just goes on a loops. Claude seems to be able to deduct the number of unique letters used in the key after I explained the encryption method to it.  It's eventually able to solve it all the way to the plaintext when I feed it more and more explicit clues (the last piece is the literal key, but it was able to guess one little bit of information encoded in the key, so I relented, lol), but the current consensus is that it only able to solve it if the ciphertext itself is longer.
