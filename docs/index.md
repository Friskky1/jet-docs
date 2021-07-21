# Information

For initial setup, see the [installation guide](installation.md).

## What is JustEmuTarkov?

JustEmuTarkov, or **JET** for short, is an [self-hosted backend server for Escape from Tarkov](https://justemutarkov.eu/). It has the capability to host a backend server locally on your network, so you can play EFT on your own terms. This means you can modify almost every serverside parameter you want, and play exactly how you want. This includes a robust modding system, which allows you to tweak your game as you see fit.

JET Server supports modding which allows you to edit server behaviour or database's without touching them.

JET works by emulating BSG's production backend, which is a RESTful API used to provide data to your game to allow it to talk to BSG's servers. We emulate that API, and allow you to both host the backend, and modify it to your heart's content. This gives you the power to modify anything that BSG would normally provide on their backend, such as raid parameters and user profile stash. You can give yourself 900 million roubles, create your own weapons and items, turn all scavs into Killas, etc. Currently, JET is written in [Node.js](https://nodejs.org/), with the internal `http` module.

JET Server is *not* a cheat, and *not* a multiplayer server. It is strictly an endpoint for your game to talk to, to receive important information that allows the game to run entirely offline. This means there is no match server, and therefore, no way to play with your friends. Since it is a locally hosted backend, this also means it has no connection to your BSG account, your EFT profile, or anything to do with BSG's representation of your copy of the game. This means you *cannot* use JET as a way to cheat in items or money to your online account. It is entirely localized on your host computer.

To prevent our modified client files from leaking into your live EFT installation, we implore that you do not mix JET files with your normal EFT installation. It is recommended to create a separate directory for your JET client, meaning you would have two separate installations of the game. This way, it is impossible to get banned for client modifications, since you would never be launching into BSG's servers with your JET-only installation. BattlEye is also disabled and removed from JET, which would prevent you from running the live game using your JET install.

If you have more questions about EmuTarkov/JET, you should join one of the two Discord servers below:

- [JustEmuTarkov Discord](https://discord.gg/T66tGKa)
- [EmuTarkov Community](https://discord.gg/NJANk5gCeN)

Partnered communities:

- [ConfigFreaks Discord](https://discord.gg/CeBQqzB)
- [Kovacs' Altered Escape Discord](https://discord.gg/tagQAqw3HB)

## Other Links

- [Multi Version & Language Item Search Engine](https://eft.justemutarkov.eu/)
- [Self-Hosted Git](https://git.justemutarkov.eu/) _(if you want access, open a ticket on the [JustEmuTarkov Discord](https://discord.gg/T66tGKa))_
- [JET Download Center](https://justemutarkov.eu/download)

## Footer

For queries on this documentation, email [kio@is.dead.gg](mailto:kio@is.dead.gg).
