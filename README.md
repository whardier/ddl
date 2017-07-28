# Differential Document Ledger (DDL)

Concensus oriented ledger system to quickly and efficiently distribute persistent and ephemeral data between backend data providers and frontend services.

## Use Case

Use DDL to replicate channel based (not pub/sub.. but not not pub/sub) documents for high uptime, low latency applications.  Client libraries modify local storage on demand and 'catch-up' to full snapshots.

My (Shane) initial use case is to send log files as well as a large JSON structure through DDL while allowing client feedback.  This is an interesting and possibly useful approach to handle online markets (crypto/stocks/beenie babies/...)

## Goals

Take structured content and let several large nodes handle differential compression and analysis until there is a concensus and storage requirements are met.  Allow programming libraries to send full of partial document updates.
