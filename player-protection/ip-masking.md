---
description: Preventing servers from seeing your real IP when you connect to them
icon: masks-theater
---

# IP Masking

Typically, when connecting to a server, the server console would print out your IP address as you connect to it. For example, let's say the user **md5nake**'s IP is 127.0.0.1. Then the server console would output:

```
[16:14:12 INFO]: UUID of player md5nake is 12ff72a5-13a7-4d42-a41f-999466d64097
[16:14:12 INFO]: md5nake joined the game
[16:14:12 INFO]: md5nake[/127.0.0.1:44290] logged in with entity id 77 at ([world]7.5, 111.0, -5.5)
```

As knowing a player's IP address allows for DDoS attacks, as well as knowing one's approximate (city/region-level) location, MineKeep employs a hashing algorithm when forwarding player IPs to user servers. This preserves the identity aspect of an IP (e.g allowing alt detectors and /ban-ip to function), whilst protecting the privacy of the player. Here's an example of a masked/hashed IP:

```
[16:14:12 INFO]: UUID of player md5nake is 12ff72a5-13a7-4d42-a41f-999466d64097
[16:14:12 INFO]: md5nake joined the game
[16:14:12 INFO]: md5nake[/123.123.123.123:0] logged in with entity id 77 at ([world]7.5, 111.0, -5.5)
```

In summary: Player IP addresses are not forwarded to user servers.
