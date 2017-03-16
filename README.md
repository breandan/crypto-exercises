## How to Share a Secret Message

##### What’s a secret? Something meant to be kept unknown or unseen by others.

> ***se·cret /ˈsēkrit/***

> *adjective*

> 1. not known or seen or not meant to be known or seen by others. ("how did you guess I had a secret plan?")

> *noun*

> 1. something that is kept or meant to be kept unknown or unseen by others. ("a state secret")


##### Let’s say you have a secret. How you make sure your secret stays secret?

* Do not write it down. (Even in your diary.)
* Do not talk about it. (Even in your sleep.)
* Do not record it. (Even on your smartphone.)

##### What if you need to share the secret? How can we share a secret safely?

* We need to turn the secret into a message.
  * How do we write (or encode) this message?
  * How do we read (or decode) this message?
  * How do we keep our message safe?
* We can share the message in person.
  * How do you know you are alone?
  * Is the other person really your friend?
  * What if your friend lives far away?
* We can share the message in public.
  * Strangely, this is the safest way to share a secret. Requires that we be very careful.
  * If you need to share a secret message, it’s safest to assume everyone can read it.
  * How do we prevent others who read our message from understanding the contents?

```
Exercise #1: Let’s encode a message!

There are many ways to encode messages.
Computers often use numbers to represent characters.
We can think of a message as a long list of numbers (or one really big number).
```

##### How can you share a secret in public without sharing the secret?

* We can hide the secret in a secret place
  * How do we share the location of this place?
  * Can we be sure that no one is watching us?
  * What if someone finds out our hiding spot?

* We can hide the secret in plain sight
  * This technique is called [steganography.
  * What happens if someone is observant?
  * What if someone learns our technique?

* We can use a language only we understand.
  * How can we be sure no one else listening can understand our language?
  * What if someone else can read our language? They will know our secrets!
  * What if someone else can write our language? They can change our messages!

* We can scramble up the message somehow.
  * How do we scramble or (encrypt) the message?
  * How do we unscramble or (decrypt) the message?
  * How do we keep the message secret?

Exercise #2: Let’s write a cipher!

* What is a substitution cipher?
  * Substitution ciphers are (weak) encryption schemes.
  * They work by replacing symbols and words (or Strings) with other symbols.
  * Ciphers must be reversible (when reversed they produce the original message)

* What are some substitution ciphers?
  * Codepoint cipher
  * Caesar cipher
  * Isogram cipher

* What is the difference between encoding and encryption?
  * Substitution ciphers are just a fancy encoding mechanism.
  * Encryption is an encoding that is difficult to decode.

##### How safe are substitution ciphers?

* How do we communicate using ciphers?
  * We need to agree on a common method (protocol).
  * We need to agree on a common secret (key).
  * How do we agree on a common secret? Back to square one.

* What are the risks of using this kind of cipher?
  * What happens if someone guesses our protocol? They still need to guess the key.
  * What happens if someone deciphers a single message? They learn they key.
  * What happens if someone learns our key? They can break every message.

```
Exercise #3: Let’s break a cipher!

Why are substitution ciphers dangerous?
If someone learns a plaintext ciphertext
They work by replacing symbols and words (or Strings) with other symbols.
Ciphers must be reversible (when reversed they produce the original message)

* What is the only way to guarantee an unbreakable cipher?
  * One-time pad
````

#### crypto-exercises

Here we demonstrate some simple ciphers and how to break them. This repository contains sample code, implementing the following ciphers:

* [Caesar cipher](https://en.wikipedia.org/wiki/Caesar_cipher)
* [Isogram cipher](https://en.wikipedia.org/wiki/Isogram#Uses_in_ciphers)
* [Mixed alphabet (random) cipher](http://crypto.interactive-maths.com/mixed-alphabet-cipher.html)
* [One-time pad](https://en.wikipedia.org/wiki/One-time_pad)

Exercises can be compiled and run using [Gradle](https://gradle.org/), or with [IntelliJ IDEA](https://www.jetbrains.com/idea/).

## Building

First ensure [JDK 1.8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) and [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) are installed and run the following command in your terminal.

```
git clone https://github.com/breandan/crypto-exercises && cd crypto-exercises && ./gradlew runIdea
```

After several minutes, a program called "IntelliJ IDEA" should start. If you receive an error, make sure JAVA_HOME is [correctly set](https://docs.oracle.com/cd/E19182-01/820-7851/inst_cli_jdk_javahome_t/). Once the program loads, right click on the file called *HelloCrypto.kt* and select "Run". You should see the following output.

```
Let's learn about cryptology!
```
