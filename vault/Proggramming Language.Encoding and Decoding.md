---
id: 0nEePlwY9ymdUErRVqIJZ
title: Encoding and Decoding
desc: ''
updated: 1641330033261
created: 1641328707436
---

> This notes are copied from several sources, including wikis, blogs, etc

## Why is used:

Encoding and Decoding schemes are commonly used when there is a need to encode binary data that needs to be stored and transferred over media that are designed to deal with ASCII.

## Types 

There are several schemes for encoding and decoding, the most used are `base32` and `base64`.

### Base32

Base-32 numeral system. It uses a set of 32 digits, each of which can be represented by 5 bits (25). One way to represent Base32 numbers in a human-readable way is by using a standard 32-character set, such as the twenty-two upper-case letters A–V and the digits 0-9.

**Advantages:**:

* The resulting character set is all one case, which can often be beneficial when using a case-insensitive filesystem, DNS names, spoken language, or human memory.
* The result can be used as a file name because it cannot possibly contain the '/' symbol, which is the Unix path separator.
* The alphabet can be selected to avoid similar-looking pairs of different symbols, so the strings can be accurately transcribed by hand. (For example, the RFC 4648 symbol set omits the digits for one, eight and zero, since they could be confused with the letters 'I', 'B', and 'O'.)
* A result excluding padding can be included in a URL without encoding any characters.
* Base32 representation takes roughly 20% - 21% less space. (1000 bits takes 200 characters, compared with 250 for Base16).

**Disadvantages**:

* Base32 representation takes roughly 20% more space than Base64. Also, because it encodes 5 bytes to 8 characters (rather than 3 bytes to 4 characters), padding to an 8-character boundary is a greater burden on short messages.

### Base64

**Advantages:**:
* Uses less space compared to base16 and base32.
* Used to transport larger binary data, in ASCII format and smaller footprint.

**Disadvantages**:
* More complex to decode, and it is also case sensitive.

## Optimization to save binary files online.

There are several sofwares that will encode your images and other binaries files and help you to add it into your html. This is not always a good idea because as mention above when we are encoding data most of the time it will increase the size of the data by 25%. This will not only lead to bigger data, also higher download time.

Another important factor is the CPU overhead, since the data is coming encoded the CPU needs to decode all the images/data taking also some of the resources of the machine.

Cahching Issues are also present since when a user access a website the images, and other types of binary data are saved into a cache to be displayed later on. Meaning a higher file size will not be beneficial in these cases.

**Other cases**: Some times it is a good idea to use encoded data in places where the link is bigger than the actual `base64` data. This will also include logos,and small images and helps the recipient not deal with permissio queries to download by email client.



