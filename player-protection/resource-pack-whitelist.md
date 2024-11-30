---
icon: list-check
description: Preventing side-channel IP leakage
---

# Resource Pack Whitelist

When a server sends a resource pack request packet to a client, the client will send an HTTP request to whatever URL the server says the resource pack is hosted at. Because those URLs can be attacker-controlled, a server owner would be able to extract the IP address of any client accepting the server's resource pack.

MineKeep prevents IP leakage from happening this way by employing a resource pack host whitelist. Resource pack requests can only reference packs hosted on a set list of trusted domains. All other requests will be dropped.

Here are the whitelisted domains:

* \*.server.minekeep.gg ([self-hosted packs](../opening-http-ports.md))
* download.mc-packs.net (mc-packs)
* drive.usercontent.google.com (Google Drive)
* github.com (GitHub)
* raw.githubusercontent.com (GitHub)
* atlas.oraxen.com (Oraxen)
* nauticalhosting.org (NauticalRanks)
* lobfile.com (ItemsAdder)

If you need to serve a resource pack. Make sure it originates from one of these domains.
