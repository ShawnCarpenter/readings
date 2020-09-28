# Auth, passwords, and encryption

Usually you want encryption to be fast so people use it. Password hashing is a special case where you want it to be slow because that makes brute-force attacks more time consuming. Bcrypt slows down the hashing process.

NEVER store plain text passwords.

There is a library for using bcrypt in node, use it, don't try to make your own encryption.

