# Privacy Policy

This Privacy Policy explains how filteringdev-noti (the "Service") processes information when you use the Service through Discord or Telegram.


## 1. Information processed

The Service processes the following categories of information to provide release notifications:

- **Platform and destination information:** Discord or Telegram platform type; channel, chat, or user identifier; Telegram forum topic identifier where applicable; Discord server identifier; and the identifier of the user or administrator associated with a destination.
- **Subscription and preference information:** subscribed repository, language preference, prerelease-notification preference, direct-message setting, and record-creation timestamp.
- **GitHub repository and release information:** GitHub App installation and repository information; repository owner and name; release ID, publication timestamp, name, tag, body, author, URL, prerelease status, and target commit. Draft releases are ignored.
- **Delivery information:** destination identifier, release key, delivery status, error message, and timestamp of each delivery attempt. A release key combines a repository and release ID.
- **Release deduplication and polling information:** repository, release ID, receipt timestamp, last processed release publication timestamp, HTTP ETag, and watermark update timestamp. This information prevents duplicate notifications and supports efficient polling.
- **Operational logs:** service configuration, database and platform-notifier startup, GitHub App installation refreshes, release polling and processing, selected destination counts, and delivery failures. Delivery failures may include a destination identifier, platform, release key, and error message.

The Service does not need your Discord or Telegram password. Authentication tokens and other service secrets are managed separately from the above user records.

## 2. How information is used

The Service uses information to:

- store and manage subscriptions and notification preferences;
- identify an authorized Discord or Telegram destination and send release notifications;
- retrieve releases from repositories where the GitHub App is installed, and process, retry, and prevent duplicate release notifications;
- record delivery results, diagnose failures, protect the Service, and maintain its operation; and
- respond to deletion requests made with the `/forget` command.

## 3. Storage and security

Service records are stored in a SQLite database. The underlying implementation exports database changes atomically and configures the database file with owner-only read/write permissions. The Service authenticates GitHub API access through a GitHub App and polls installed repositories for releases, using HTTP ETags where available to avoid retrieving unchanged release lists.

No method of storage or transmission is completely secure. The operator cannot guarantee absolute security.

## 4. Disclosure and third-party services

To provide the Service, information is exchanged with the relevant third-party platform:

- Discord receives the notification content and destination information needed to deliver messages to Discord.
- Telegram receives the notification content and destination information needed to deliver messages to Telegram.
- GitHub provides GitHub App installation, repository, and release information used to process notifications.

Discord, Telegram, and GitHub process information under their own terms and privacy policies. The Service does not sell personal information.

## 5. Retention and deletion

The Service does not promise an automatic time-based deletion schedule. Subscription records, preference records, delivery-attempt records, operational logs, release-receipt records, and release-watermark records may be retained until deleted or otherwise removed by the operator.

You may use `/forget` in Discord or Telegram to request deletion. For a server or group, this removes subscriptions and delivery history associated with that server or chat. For a direct message, it removes subscriptions, delivery history, and the applicable language setting. Release-receipt and release-watermark records are not linked to a user or destination and are not removed by `/forget`.

The Service does not provide a data-export feature.

## 6. Your choices

You can stop using the Service by removing it from your Discord server, leaving or deleting a Telegram chat as applicable, or no longer interacting with the Service. Removal from a platform does not itself delete stored records; use `/forget` for deletion of the records described above.

## 7. Changes to this Policy

The operator may update this Privacy Policy. The updated version takes effect when posted unless a later effective date is stated. Continued use of the Service after the effective date means that you acknowledge the updated Policy.


For the Korean version, see [PRIVACY_POLICY-ko.md](PRIVACY_POLICY-ko.md).