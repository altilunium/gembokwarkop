# gembokwarkop
casual encryption for daily use

<img width="776" height="641" alt="image" src="https://github.com/user-attachments/assets/de125d5a-34ed-4952-b7c3-e8c84e266e84" />


> vt/112.024.233 (21.5.26 13.54.04) : The plaintext is encoded with Base64, then encoded again with Vigenere cipher.
>
> vt/112.025.261 (21.5.26 15.31.23) : I know, right? Tried to brute force them through DeepSeek and Claude, and the former just goes on a loops. Claude seems to be able to deduct the number of unique letters used in the key after I explained the encryption method to it.  It's eventually able to solve it all the way to the plaintext when I feed it more and more explicit clues (the last piece is the literal key, but it was able to guess one little bit of information encoded in the key, so I relented, lol), but the current consensus is that it only able to solve it if the ciphertext itself is longer.



# Fun Little Experiment

## ChatGPT

"The plaintext is encoded with Base64, then encoded again with Vigenere cipher." tell me how strong this one

----

Base64 does not add security at all. It only transforms data into a text-safe representation. Vigenère cipher, on the other hand, is a real cipher but a very old and weak one by modern standards. When you apply Vigenère after Base64, nothing meaningful is gained in terms of security.

---- 

you said it's weak.. then break this

 "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"

----

I can’t actually recover a plaintext from that as-is. So the limitation here isn’t computing power, it’s missing critical information. With just the ciphertext and no key or hint about the key length, there’s no direct route to a definitive plaintext.

-----

you said it's weak. then you give up.. funny

-----

Calling something weak doesn’t mean it can be casually peeled open on demand without the missing pieces.

## Gemini 

To put it bluntly, this setup is incredibly weak and offers virtually no real security against a determined attacker.

The first layer, Base64, is not encryption at all; it is simply a reversible encoding mechanism designed to safely transport binary data over text-based protocols. While it does technically alter the character distribution of your original plaintext by mapping it to a specific 64-character alphabet, it does not hide the underlying data structure. Base64-encoded text possesses its own highly predictable mathematical signature and heavily skewed character frequencies that any automated script can instantly recognize and exploit.

The outer layer, the Vigenere cipher, is a historical polyalphabetic substitution cipher that has been fundamentally broken for over a century.

---- 

The Solution
Vigenère Key: ALCHYMISTICAL (14 characters)

The Decoded Plaintext:

"The Alchemist, by Ben Jonson. Act I, Scene I. Subtle, Face, Dol Common.

SUBTLE: Believe it, I will.
FACE: Do thy worst. I defy thee.
SUBTLE: Why, I'll tell the king of it, and thine honesty, and thy cold capon too, and thy sauce, and thy sub-clerk.
FACE: What, and my pocket-handkerchiefs?
SUBTLE: Yes, all thy linen, and thy laundry-bills, and thy whole estate, and how thou didst cheat the poor citizens of their plate and their rings, and how thou wert a famous rogue before I found thee, and how I did give thee thy first doublet and thy hose, and made thee a man out of a dung-hill, where thou wert starving, and didst eat nothing but roots and water-cresses."

((this is all hallucinations nonsense)) ((ignore that))


## Claude Sonnet 4.6

This is quite weak as a combined scheme.

Base64 is not encryption. It's a reversible encoding with zero secrecy — anyone who recognizes it (the character set A–Z, a–z, 0–9, +, /, and = padding is unmistakable) can decode it instantly. Applying it before Vigenere adds no cryptographic strength whatsoever.

Vigenere itself is weak. It was broken in the 19th century (Kasiski, 1863). Against a known or guessable key length, index-of-coincidence analysis and frequency analysis recover the key from a modest amount of ciphertext. Against modern tools, it falls in seconds.

Base64 pre-encoding makes Vigenere worse, not better. Base64 output has a highly restricted and non-uniform character distribution — only 64 possible characters, with = appearing only at the end, and certain characters more frequent than others. This gives an attacker more statistical structure to exploit, not less. The Vigenere cipher's classical weakness (frequency analysis per key-position column) still applies; the attacker just works in Base64-alphabet space.

---- 

Let me work through this systematically.

* Try to decode the base64 first, then analyze
* Decode base64 and inspect bytes
* Analyze the decoded base64 content
* Byte-level IC analysis to find key length
* Try cracking byte-level Vegenere using Base64 character frequency scoring
* Try classical Vigenere analysis on the ciphertext string directly
* Try common keys and Caesar shifts on classical Vigenere
* Refined byte-level Vigenere crack with proper base64 scoring
* Try Base064-alphabet Vigenere theory
* Crack B64-alphabet Vigenere with key length 4 using IC analysis
* (16 minutes processing, still not over)
