# Blockstack-Social-Key-Recovery

## Description
Repo is intended for a proof of concept for an implementation of Social Key Recovery in Blockstack (https://www.blockstack.org).

Blockstack is a decentralized application platform that takes advantage of decentralized storage through Gaia (https://github.com/blockstack/gaia). This allows for full control of a user's files, where they are stored (Azure, Dropbox, personal server, etc), and how they are stored (encrypted or public).

When a user creates their blockstack ID for the first time, they generate a seed that is used as the private key throughout the app ecosystem. Using this seed allows them to recover their account if something were to happen to their computer/phone.

Unforunately, if a user loses their seed and loses access to their blockstack account, then the account is no longer recoverable. 

This draft/implentation allows one to securely share and recover their profile from a group of trusted friends. This implements the Secret Sharing scheme (https://tools.ietf.org/html/draft-mcgrew-tss-03) which allows one to recover a seed from a subset of a group of trusted parties (ex. 2 out of 3 parties). 

## UML Process
![image](https://github.com/AnthonyRonning/Blockstack-Social-Key-Recovery/blob/master/Blockstack%20Social%20Key%20Recovery.png)
