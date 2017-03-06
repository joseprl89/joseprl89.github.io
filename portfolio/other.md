---
layout: page
title: Other portfolio
---

*Note that most recent projects I have worked on are protected by NDA and I can not list them here.*

# Other portfolio

## 2 Factor Authentication proxy to internal VPN

A client had a private VPN only accessible from the infrastructure of their own clients.
In order to allow for better mobility, this project was undertaken to securely expose
to the client the servers hosted within that VPN.

The solution consisted in the creation of two web interfaces, one to manage user's access,
and another one the user would use to log in and via 2FA using a companion iOS
or Android app, and be able to access the servers he was granted access to using
our backend as a proxy.

The proxy was based on NodeJS and using a proxy library, that we had to tweak to
to correctly manage HTTP sessions between the client and the VPN host.

### Uses:

* *Bootstrap*
* *JQuery*
* *NodeJS* backend
  * *MongoDB*
  * *Express*
  * *Proxy library*

## By-Taxi fleet management site

Wrote a fleet management site for By-Taxi, where the admins could see the driver's
location, metadata on users, usage,...

### Uses:

* *Bootstrap*
* *JQuery*
* *LAMP* stack
* *Google Maps JS*

## Xen host & guest backup system

The goal of this project was to create a resilient structure for a critical
system in the industrial sector.

The solution was a web interface, installed in the Xen host, in which the user
could manage, trigger, and restore backups of the Xen guests. Furthermore, cron
jobs could be created using the web interface to automatically create the backups.

Alongside this web interface, a set of scripts were created to do the heavy-lifting
of the backup process.

### Uses:

* *Xen*
* *Bash* scripting
* *LAMP* stack
* *Rsync*
* *NFS*

## SSG4Env

SSG4Env was a EU funded project where multiple companies and universities
collaborated together to specify, design, implement, evaluate and deploy a
service-oriented architecture and middleware which would allow application
developers to build open large-scale semantic-based sensor network applications
for environmental management.

My role in this project was to integrate the architecture components and perform
stress testing on the solution.

As part of it, I published 4 documents that were hosted in its website
(no longer maintained).
