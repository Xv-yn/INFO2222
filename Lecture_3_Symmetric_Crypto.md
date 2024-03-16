# Lecture 3 Symmetric Crypto


#### Methods of Symmetric Encryption

###### One TIme Pad

Each key can only be used once. This increases security because each message's encryption is different.

```mermaid
flowchart

node1("KeyGen") -->|"Uniformly Sample"| node2("Key")

node2 -.-||"+" node3("Message")

node2 --> node4("Encryption")
node3 --> node4

node4 --> node5("Cipher Text")

```
This method can be imagined as having to use a different key every time you want to enter your house. While, this makes it hard for someone to pick the lock, it is not efficient to keep changing keys every time.

Note that it is barely usable in practice. This is because the key has to be as long as the message. Hence, This method has high security but low usability.

###### Stream Ciphers

This method to encrypt text is one where a cryptographic key and algorithm are applied to each binary digit in a data stream.

This method can be imagined as changing each letter in a message to an encrypted version.

###### Block Ciphers

A block cipher can be argued to e the 'opposite' of a stream cipher. This method uses a key and algorithm to encrypt blocks of daa instead of individual bits.



