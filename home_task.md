# Home Task

## Which place for which setting?

(a) For a quick test, I would type export NAME=value directly in the terminal.
It works immediately and disappears when I log out, so it leaves nothing behind.
(b) For a setting only for me, I would use ~/.bashrc.
It is my personal file in my home folder, and bash reads it every time I log in.
I write it as export NAME=value and use source ~/.bashrc to load it right away.
(c) For a setting for all users, I would use /etc/environment.
It needs sudo, it applies to every user on the server, and it is written as NAME="value" without export.

## Why is an SSH key safer than a password?

An SSH key is safer because it is a long random key that cannot be guessed like a password.
My private key never leaves my PC and is never sent over the network. The server only sends a puzzle that only my private key can solve.
If someone steals my private key, they can log in to my server as me without any password.
Then I should immediately remove the matching public key line from ~/.ssh/authorized_keys on the server.
After that, I should make a new key pair, add the new public key to the server, and delete the old key files from my PC.
