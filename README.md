This tutorial will introduce quries concept.
Refer URL for more info, https://hyperledger.github.io/composer/latest/tutorials/queries.html

YouTube Video, https://www.youtube.com/watch?v=zmm_TXd0o6o

These are JSON values used,

Trader
======

{
  "$class": "org.example.mynetwork.Trader",
  "tradeId": "Rahul",
  "firstName": "Jenny",
  "lastName": "Jones"
}

{
  "$class": "org.example.mynetwork.Trader",
  "tradeId": "Modi",
  "firstName": "Amy",
  "lastName": "Williams"
}


Asset
=====

{
  "$class": "org.example.mynetwork.Commodity",
  "tradingSymbol": "ABC",
  "description": "Test commodity",
  "mainExchange": "Euronext",
  "quantity": 72.297,
  "owner": "resource:org.example.mynetwork.Trader#Rahul"
}

{
  "$class": "org.example.mynetwork.Commodity",
  "tradingSymbol": "APL",
  "description": "Apple Stock",
  "mainExchange": "BSE",
  "quantity": 12.297,
  "owner": "resource:org.example.mynetwork.Trader#Rahul"
}

Transaction
===========

{
  "$class": "org.example.mynetwork.Trade",
  "commodity": "resource:org.example.mynetwork.Commodity#ABC",
  "newOwner": "resource:org.example.mynetwork.Trader#Modi"
}

