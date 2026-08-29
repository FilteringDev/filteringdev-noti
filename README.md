# filteringdev-noti
This document describes the filteringdev-noti bot, which operates on the basis of [webhook-noti](https://github.com/FilteringDev/webhook-noti).

## repositories
The bot monitors repositories where its GitHub App is installed. It refreshes the installed-repository list every 10 minutes and checks for releases every 60 seconds. After an initial baseline is recorded, the bot sends a notification for each newly published non-draft release after internal verification. Previously published releases are not sent when monitoring begins.

## Installation
Use one of the following methods to install the bot.

- Discord: Open and follow the instructions at https://discord.com/oauth2/authorize?client_id=1543001264776814723
- Telegram: `@filteringdev_noti_bot`

## Legal documents
- [Terms of Service](TERMS_OF_SERVICE.md)
- [Privacy Policy](PRIVACY_POLICY.md)

For the Korean version, see [README-ko.md](README-ko.md).
