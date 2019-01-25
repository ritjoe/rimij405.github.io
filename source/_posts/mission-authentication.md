---
title: 'Mission: Authentication'
date: 2019-01-24 22:09:42
categories:
- [blog, cybersecurity]
tags:
- tutorial
- ssh
- authentication
photos:
- /blog/cybersecurity/mission-authentication/lewis-ngugi-186309-unsplash_thumb.jpg
- /blog/cybersecurity/mission-authentication/pankaj-patel-729895-unsplash_thumb.jpg
---

# Mission: Authentication #

Today's little server-side experimentation dealt with ssh security and authentication. I'll admit, I've been logging into my personal server using a password.

Before we dive into it, as a **disclaimer**:

> **I am in no way a cryptologist, cryptographer, or security expert. The material written here was taken from around the web, and, as all things, is subject to human error.**

That [cleartext](https://simple.wikipedia.org/wiki/Cleartext) security information has been passing through my tunnels ever since I started working on that server. It was simply time to move one step up in the world of authentication - it was time to use some *cryptography*.

## Overview ##

As always, I like to make sure I understand what it is I'm playing with. Cryptology? Cryptography? Aren't they the same thing?

Well, according to [@SEJPM](https://crypto.stackexchange.com/users/23623/sejpm) and [*@Lery*](https://crypto.stackexchange.com/users/29574/lery) over at the Crypto StackExchange, there are a couple of related terms that tend to be used [interchangeably](https://crypto.stackexchange.com/questions/57818/is-there-any-difference-between-cryptography-and-cryptology).

### Semantics ###

To get down to the semantics:

> *Cryptology* is the study of cryptography (Definition 1.1) and cryptanalysis.

In other words, it's referred to as the, "science of cryptography."

> *Cryptography* is the study of mathematical techniques related to aspects of information security such as confidentiality, data integrity, entity authentication, and data origin authentication.

Cryptography deals with the actual security, in practice. There's also one other term:

> *Cryptanalysis* is the study of mathematical techniques for attempting to defeat cryptographic techniques, and, more generally, information security services.

That's where the techniques are used to evaluate cryptographic practices. It's good to keep these things in mind when we talk about modern cryptology.

### The Past ###

While the actual study of the practice is relatively young - [within 100 years, according to Huzaifa Sidhpurwala](https://access.redhat.com/blogs/766093/posts/1976023) - cryptography itself has been around for thousands of years. The encryption of messages by hand have been used to keep sensitive secrets away from prying eyes; one of the earliest known and simplest ciphers in history is known as the [Caeser cipher, or substitution cipher](http://practicalcryptography.com/ciphers/caesar-cipher/). It took it's name from Julius Caeser who used it to keep military communications secret.

### The Now ###

Security on the interet, in some ways, hasn't changed. We still encrypt our text and we still rely on messages that travel between endpoints. Today we use public-key cryptography, or asymmetric cryptography, in various sceruity models ranging from authentication, authorization, and more.

## Authentication ##

When our client reaches out to our server/host, one crucial part in the step is to authenticate both parties.

### Client-Side ###

On the client-side, this might look like a host key fingerprint. By keeping track of this information, the client can verify that the host on the other side of the connection is, in fact, who they say they are.

### Server-Side ###

If the server is given a public key by the client, it can check to ensure the client has the accompanying private key whenever it connects. If the key is given passphrase protection, the client is responsible for authenticating the key before it can be trusted by the server as well!

## SSH ##

Secure Shell (SSH) is a cryptographic [remote login program](https://man.openbsd.org/ssh.1), providing a secure channel over an unsecured network in client-server architecture. We can use applications that leverage this protocol to do things like manage files remotely, update repositories, and transfer files.

{% asset_img pankaj-patel-729895-unsplash_large.jpg Screenshot of GitHub ssh session - Image by Pankaj Patel %}

One strategy for securing this channel is through the use of the public-key cryptography. With great power comes great responsibility: the ability to execute command remotely is great for DevOps and sysadmins, but, the remote communication can be exposed to a lot of third-party actors.

**PasswordAuthentication**

Logging into a secure shell remotely can vary depending on the host's settings, but, for the most part, clients typically connect to a host by providing a username, hostname, and port. The most basic of authentication allows users to enter a password (that is sent as cleartext) over the network. While this is the easiest way to remote login to a server, it's also the least secure.

**ChallengeResponseAuthentication**

Similar to PasswordAuthentication, users have to enter a password through a keyboard-interactive terminal in order to successfully authenticate their client to the host. Unlike PasswordAuthentication, this Authentication protocol can vary in security. Sometimes known as the [Challenge-Handshake Authentication Protocol](https://en.wikipedia.org/wiki/Challenge-Handshake_Authentication_Protocol) (CHAP), the host issues a challenge to the client. Once received, the client will combine that challenge with a secret that's shared between them - this is usually the password - and calculate a hashed value from it, before sending that value back to the host. The host, which should have the expected shared secret already stored, will calculate the expected value on its end before comparing it to the response from the client. If the challenge is successfully met (meaning the user input the correct shared secret), the authentication is considered successful. Some versions will allow the host to send new challenges to the client at random intervals to continually check the authenticity of the client.

### Key Fingerprints ###

In public-key cryptography, a public key fingerprint is a short sequence of bytes used to identify a longer public key. Fingerprints are created by applying a cryptographic hash function to a public key. Since fingerprints are shorter than the keys they refer to, they can be used to simplify certain key management tasks.

These keys are meant to be human readable for the purposes of identification: often public keys will be encoded into hexadecimal strings like below:

`43:51:43:a1:b5:fc:8b:b7:0a:3a:a9:b1:0f:66:73:a8`

Fingerprints won't always look like the MD5 hash above. SHA-1 fingerprints are often nothing more than a string of hexadecimal digits: `2fd4e1c67a2d28fced849ee1bb76e7391b93eb12`.

### ssh-keygen ###

`ssh-keygen` is a command line tool that [generates, manages, and converts authentication keys](https://man.openbsd.org/ssh-keygen.1) for SSH. Keys generated with this tool default to the OpenSSH-specific format. Generally, a user will generate the public key and indicate where to store the private key, before protecting them with a passphrase. While the names can be changed, in the OpenSSH format, private keys are stored in plaintext without a file extension and public keys are given the, '.pub' file extension. Although they are stored in plaintext, the data held inside them is a mix of randomly generated content based on an crpytographic algorithm. Knowing the content of one file in isolation does little to risk the host as they can easily be revoked. (This does, however, require the sysadmin know of a breach).

The tool can also be used to check the fingerprints of certain keys! Host keys are created without a passphrase as they serve as identity markers more so than authentication checks.

The following command takes a public host key created with the ED25519 algorithm, and outputs the fingerprint as an MD5 hash:

`ssh-keygen -l -E md5 -f ssh_host_ed25519_key.pub`.

By default, the fingerprint command will display a SHA256 hash:

`ssh-keygen -lf ssh_host_ed25519_key.pub`

Knowing how to get a particular formatted hash is important when checking if a host's fingerprint has changed.

### PuTTY ###

One method for setting up SSH Public-key cryptography is with [PuTTY](https://www.putty.org/), a terminal emulator that can act as a client for SSH, Telnet, rlogin, and raw TCP communication protocols.

PuTTY is joined by a few additional applications that are often run in its suite, such as PuTTYgen, an asymmetric cryptography key generation utility. Their application allows you to generate a public and private key for use in the system. In this case, private keys can be exported to the open-source OpenSSH format or as a PuTTY Private-key (*.ppk) file, a propriatary format.

You can also control the host key algorithm preference when authenticating to a host for the first time. If a client doesn't have a key in one algorithm, it will move onto the next algorithm in the preference list.

### ssh-agent ###

The `ssh-agent` is a program that [holds private keys used for public-key cryptography authentication](https://man.openbsd.org/ssh-agent.1). Initially, a system's ssh-agent will not have any private keys, but, as users `ssh-add` private keys to the client, they'll be able to authenticate automatically when the host requests their key.

The general process is to generate both a public and private key, before placing the public key on the host. The client keeps track of the local private key and presents it upon SSH login to a remote host. When the host uses the public key to request the private key, if the client does not have the private key, times out, or cannot enter the correct passphrase after a set amount of attempts, the authentication process will fail.

## Final Thoughts ##

Certifications on the Secure Socket Layer and Secure Shell logins both require public-key cryptography in order to remain secure. These algorithms are not bullet proof, but, they can take a very long time to brute force and crack.

At the end of the day, keys are generated in a pseudorandom process; it will always remain theoretically possible to crack algorithmic security systems, so long as there is an infinite amount of time and processing power.

That shouldn't scare you from securing your server and your platforms! It is unrealistic to expect anyone to crack the toughest of algorithms (short of an unknown backdoor exploitation) within any sort of reasonable amount of time, in today's age of technological dreams.

While I'm not new to being a system admin for Linux-based servers, I am paying more attention to the security that protects my data and information. You should too!