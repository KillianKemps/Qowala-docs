# Technical overview \[DRAFT\]

## Which technology to use to allow communication inside Qowala?

### 1. Matrix protocol

[Matrix](https://matrix.org) is an open standard for decentralised persistent communication. In summary, it aims to be the next generation protocol against IRC, XMPP and co.

Several server implementations already exist, among them the official one, [Synapse](https://github.com/matrix-org/synapse) is under Apache license and written in Python.

Furthermore, there are the [Vector](https://vector.im/) clients for web, iOS and Android written by the same team, with nice interface which are also under Apache license.

So, Qowala could base itself on the Matrix technology and Vector clients to have rapidly a working internal communication system. Moreover, as the protocol is entirely open, people using Qowala could easily communicate with other Matrix clients too.

There are Matrix Bridges which exist to allow to communicate between Matrix and IRC and between Matrix and XMPP for example. Qowala could maybe just be some kind of Matrix bot and develop the necessary Matrix Bridges without having to develop a special client.

**Pros:**

* New protocol which should help to compensate issues with older protocols. See the [comparison](https://matrix.org/docs/guides/faq.html#what-is-the-difference-between-matrix-and-irc).
* Already a quite usable base using modern technologies
* [Matrix's vision for users](https://matrix.org/docs/guides/faq.html#what-does-this-mean-for-users) is the same as Qowala
* Community is growing well. Benefiting exposure from the [Decentralized Web Summit](https://matrix.org/blog/2016/05/24/next-up-the-first-decentralized-web-summit/)

**Cons:**
* Even though Matrix has been initially released in [September 2014](https://matrix.org/docs/guides/faq.html#why-arent-you-doing-this-through-the-ietf-or-w3c-or-3gpp), and is working quite well, we are currently not sure if this protocol will really have success
* Matrix is currently built mainly by VoIP professionals and some other contributors. There is no global organisation like W3C or IETF to ensure this standard will be used worldwide. However, they plan to work with an official standard once they find it mature enough.

## What to use to easily integrate lots of social networks and communication services?

