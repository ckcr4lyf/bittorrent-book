# Introduction

This book aims to explain how BitTorrent works at a technical level. The first part will cover the networking/protocol at a high level with analogies, and the second part will go a bit more in depth.

## Who is this for?

People who are curious about how BitTorrent works, and are not satisfied with some generic high level defintion like "it works by sharing files via p2p" - but rather how these connections are established, how files are requested, and how we even find the peers in the first place.

I once had all these questions, and spent a lot of my time learning about it from various sources. This is my attempt to combine all that knowledge and present it in a noob-friendly way, yet detailed enough to satisfy a somewhat slightly deeper curiosity.


## Prerequisites

A little bit of familiarity with torrents would be beneficial. Not on the technical side, but experience having used them - for instance adding a `.torrent` file to a client, seeing it slowly start downloading, and finally have the completed files on your disk.

On the technical side, the first part doesn't need much background, and any terms will be explained. However for the second part, which goes in a bit deeper, it is recommended to know how HTTP requests work, what IP addresses are, what TCP is, and what hash functions are. Finishing the first part should answer most of these. Just a basic understanding at a high level is enough, knowing the ins and outs of the protocols are definitely not required.

As an example, the technical section may include language such as "The client makes an HTTP request to the tracker, which returns a list of peers - their IP addresses and ports, which the client can use to initiate a TCP connection."
