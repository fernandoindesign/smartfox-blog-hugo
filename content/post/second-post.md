---
title: "Second Post"
date: 2021-10-11T03:15:25-04:00
draft: false
categories: "web3"
author: "Robin Hood"
---

web3.eth.Iban
The web3.eth.Iban function converts Ethereum addresses from and to IBAN and BBAN.

Iban instance
This instance of Iban.

> Iban { _iban: 'XE7338O073KYGTWWZN0F2WZ0R8PX5ZPPZS' }
Iban contructor
new web3.eth.Iban(ibanAddress)
Generates a iban object with conversion methods and validity checks.

Also has singleton functions for conversion like:

Iban.toAddress()
Iban.toIban()
Iban.fromAddress()
Iban.fromBban()
Iban.createIndirect()
Iban.isValid()
Parameters
String: the IBAN address to instantiate an Iban instance from.
Returns
Object - The Iban instance.

Example
var iban = new web3.eth.Iban("XE7338O073KYGTWWZN0F2WZ0R8PX5ZPPZS");
> Iban { _iban: 'XE7338O073KYGTWWZN0F2WZ0R8PX5ZPPZS' }
toAddress
Static function.

web3.eth.Iban.toAddress(ibanAddress)
Singleton: Converts a direct IBAN address into an Ethereum address.

Note

This method also exists on the IBAN instance.

Parameters
String: the IBAN address to convert.
Returns
String - The Ethereum address.

Example
web3.eth.Iban.toAddress("XE7338O073KYGTWWZN0F2WZ0R8PX5ZPPZS");
> "0x00c5496aEe77C1bA1f0854206A26DdA82a81D6D8"
toIban
Static function.

web3.eth.Iban.toIban(address)
Singleton: Converts an Ethereum address to a direct IBAN address.

Parameters
String: the Ethereum address to convert.
Returns
String - The IBAN address.

Example
web3.eth.Iban.toIban("0x00c5496aEe77C1bA1f0854206A26DdA82a81D6D8");
> "XE7338O073KYGTWWZN0F2WZ0R8PX5ZPPZS"
fromAddress