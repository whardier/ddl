# Differential Document Ledger (DDL)

Concensus oriented ledger system to quickly and efficiently distribute persistent and ephemeral data between backend data providers and frontend services.

## Use Case

Use DDL to replicate channel based (not pub/sub.. but not not pub/sub) documents for high uptime, low latency applications.  Client libraries modify local storage on demand and 'catch-up' to full snapshots.

My (Shane) initial use case is to send log files as well as a large JSON structure through DDL while allowing client feedback.  This is an interesting and possibly useful approach to handle online markets (crypto/stocks/beenie babies/...)

One example would be taking the large order book from an exchange and exporting it in full and incremental state over DDL and storing it in a differential object within client and server logic. Allowing for asyncronous object updates without websocket requirements would be a treat for everybody (polling ftw) while also .. allowing .. for websockets and protocols like zeromq.

## Goals

Take structured content and let several large nodes handle differential compression and analysis until there is a concensus and storage requirements are met.  Allow programming libraries to send full of partial document updates.

Provide callback support for updates so that providers can measure requirements properly.

## What I'd dig

I'd like to see protobuf or other object based distribution solutions put in place - differential analysis would be a pain however.
