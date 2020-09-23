# Authentication

## User information

Sensitive user information must be stored securely. It's not just the right thing to do, it's the law. User information is protected by law in many parts of the world.

## Cryptograpphy

Cryptography is the science of encoding information so that it requires a key of some sort to decipher.

## Hash algorithms

A cryptographic hash algorithm processes information in such a way that the same message is always going to result in the same hash but reversing the hashing process is very difficult. Passwords are hashed with a one way hashing algorithm before storage so that even if the password file is compromised the passwords are not easily retrievable.

## Cypher algorithms
Cypher algorithms are designed to be reversible using a secret key.

## Basic authentication

Not really secure. The username and password are encoded with base 64 encoding and sent as part of an authorization header. This is not very secure because base 64 is easily reversible.