---
description: Preventing side-channel IP leakage
icon: list-check
---

# Resource Pack Whitelist

When a server sends a resource pack request packet to a client, the client will send an HTTP request to whatever URL the server says the resource pack is hosted at. Because those URLs can be attacker-controlled, a server owner would be able to extract the IP address of any client accepting the server's resource pack.

MineKeep prevents IP leakage from happening this way by employing a resource pack host whitelist. Resource pack requests can only reference packs hosted on a set list of trusted domains. All other requests will be dropped.

Here are the whitelisted domains:

* \*.minekeep.dev ([self-hosted packs](../opening-http-ports.md))
* \*.wasabisys.com (Wasabi)
* download.mc-packs.net (mc-packs)
* drive.usercontent.google.com (Google Drive)
* github.com (GitHub)
* raw.githubusercontent.com (GitHub)
* atlas.nexomc.com (Nexo)
* atlas.oraxen.com (Oraxen)
* nauticalhosting.org (NauticalRanks)
* lobfile.com (ItemsAdder)
* dropbox.com (Dropbox)
* download\*.mediafire.com (MediaFire)

If you need to serve a resource pack. Make sure it originates from one of these domains. Also make sure that the URL you provide leads directly to the download, and not a page with a button that says download. Otherwise Minecraft does not recognise it.
