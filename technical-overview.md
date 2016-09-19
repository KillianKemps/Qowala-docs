# Technical overview \[DRAFT\]

## Which technology to use to allow communication inside Qowala?

### 1. Matrix protocol

[Matrix](https://matrix.org) is an open standard for decentralised persistent communication. In summary, it aims to be the next generation protocol against IRC, XMPP and co.

Several server implementations already exist, among them the official one, [Synapse](https://github.com/matrix-org/synapse) is under Apache license and written in Python.

Furthermore, there are the [Vector](https://vector.im/) clients for web, iOS and Android written by the same team, with nice interface which are also under Apache license.

So, Qowala could base itself on the Matrix technology and Vector clients to have rapidly a working internal communication system. Moreover, as the protocol is entirely open, people using Qowala could easily communicate with other Matrix clients too.

There are Matrix Bridges which exist to allow to communicate between Matrix and IRC and between Matrix and XMPP for example. Qowala could maybe just be some kind of Matrix bot and develop the necessary Matrix Bridges without having to develop a special client.

## What to use to easily integrate lots of social networks and communication services?

