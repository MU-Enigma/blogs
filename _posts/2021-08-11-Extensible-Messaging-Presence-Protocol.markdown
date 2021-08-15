---
layout: post
title:  "Extensible Messaging Presence Protocol"
date:   2021-08-11 12:00:00 +0530
author: "Dhathri Meda"
categories: protocols
---

XMPP was a vague term to me prior the live-stream. Then, I eventually researched about it and began to appreciate its wide usage and great potential in instant messaging applications. The protocol is decentralized, secure, and flexible. It not only supports one-to-one messaging between entities but also multi-party messaging (which enables an entity to join a chat room for the exchange of messages with several participants). The messages can be text messages embedded in XML format but XML can also be used to send control messages between entities i.e., users, bots, servers, devices etc. This architecture is very similar email, where someone on gmail.com can send an email to someone with an account on hotmail.com.

WhatsApp mainly utilizes Multi user chat (MUC) which is is an XMPP extension for multi-party information exchange similar to Internet Relay Chat (IRC), whereby multiple XMPP users can exchange messages in the context of a room or channel. In addition to standard chatroom features such as room topics and invitations, the protocol defines a strong room control model, including the ability to kick and ban users, to name room moderators and administrators, to require membership or passwords in order to join the room, etc. Because MUC rooms are based on XMPP, they can be used to exchange not only plaintext message bodies but a wide variety of XML payloads.

XMPP is quite unique since you can create an account on the client and it will push it through and create it on the server. So, we don’t have to log into the server to do it. Hence, we can host our own server using XMPP. It dosen't just allow us to communicate with people that are on the server with the same IM service but it also allows servers to communicate with themselves creating a global federated network. For creating our own XMPP servers, we can choose server softwares such as ejabberd and Prosody. These support server-to-server connections. All we need for creating our own XMPP server are pubic domain name, public IP address and a port open in your firewall.

WhatsApp uses ejabberd with a FreeBSD operating system. It is scalable, optimized for mobile needs, friendly to high-load systems, and has little downtime. Ejabberd has a great degree of customization and modularity. The server offers high security with SSL/TLS encryption.
