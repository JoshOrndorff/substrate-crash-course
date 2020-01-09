Structure of a Substrate Node
=============================

A blockchain node has many jobs. Taking a simple cryptocurrency as an example:
* Accept transactions from users
* Gossip transaction to and from other nodes
* Ensure no transaction spends more tokens than the user has
* ensure no transaction spends another user's tokens
* Discover peers on startup and continually

I nSubstrate, there is the outer node and the runtime.

[Diagram]

The runtime houses your business logic --the stuff that makes your blockchain unique.
The outer node is responsible for all the stuff that all blockchains need to do: peer discovery, gossiping blocks, gossiping transactions, creating blocks, deciding which chain is canonical.

Having this clear distinction between the runtime and the outer node allows a few cool things.
Like runtime upgrades.
And not needing to re-write all the common stuff.

In general, you can write a runtime however you like. You can use any programming language, you just have to implement the right APIs. In this course we'll stick to using rust and FRAME, Parity's framework for composing runtime's out of individual units called pallets.

[Daigram]

FRAME-based runtimes can easily include or exclude whichever pallets they like. Substrate comes with many useful pallets already, and you can always write your own as well. We'll write our own pallet in the next unit. To get our feet wet, let's start by removing a pallet.

TODO explain how to remove the template pallet.
