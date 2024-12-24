---
icon: globe
description: Exposing HTTP services from a running server instance
---

# Opening HTTP ports

Sometimes one needs to run an HTTP server on their Minecraft server. Perhaps in order to self-host a dynamically generated resource pack (with ItemsAdder for example), or perhaps in order to expose a Dynmap instance to the internet.

MineKeep allows user servers to listen on the following ports:

* 2053
* 2083
* 2087
* 2096

### Example

If your server's name is "example" and you've configured Dynmap to listen on port 2053, then your map will be available on [https://example.minekeep.dev:2053](https://example.minekeep.dev:2053). The URL will only work whilst your server is online.
