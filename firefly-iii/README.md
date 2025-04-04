# Home Assistant Community Add-on: Firefly-III

[![Release][release-shield]][release] ![Project Stage][project-stage-shield] ![Project Maintenance][maintenance-shield]

Fork of [hassio-addons/addon-firefly-iii][hassio-firefly] project
in hope of continuing to maintain this add-on.

"Firefly III" is a self-hosted financial manager. It can help you keep track of
expenses, income, budgets and everything in between. It supports credit cards,
shared household accounts and savings accounts. It’s pretty fancy. You should
use it to save and organise money.

Further information can be found at [Firefly-III].

You can also read the [full add-on documentation][docs].


## Installation

To install this add-on do the following steps:

1. On supervisor -> add-on go to the options and select Repositories.
1. Add the URL for my addons repo (<https://github.com/coostax/ha-addons.git>)
   to the add text box and click on ADD.
1. Search for the "Firefly-III" add-on in the add-on store and install it.
1. Start the "Firefly-III" add-on.
1. Check the logs of the "Firefly-III" add-on to see if everything went well.

## Configuration

**Note**: _Remember to restart the add-on when the configuration is changed._

Example add-on configuration:

```yaml
log_level: info
ssl: false
certfile: fullchain.pem
keyfile: privkey.pem
```

**Note**: _This is just an example, don't copy and paste it! Create your own!_

### Option: `log_level`

The `log_level` option controls the level of log output by the addon and can
be changed to be more or less verbose, which might be useful when you are
dealing with an unknown issue. Possible values are:

- `trace`: Show every detail, like all called internal functions.
- `debug`: Shows detailed debug information.
- `info`: Normal (usually) interesting events.
- `warning`: Exceptional occurrences that are not errors.
- `error`: Runtime errors that do not require immediate action.
- `fatal`: Something went terribly wrong. Add-on becomes unusable.

Please note that each level automatically includes log messages from a
more severe level, e.g., `debug` also shows `info` messages. By default,
the `log_level` is set to `info`, which is the recommended setting unless
you are troubleshooting.

### Option: `ssl`

Enables/Disables SSL (HTTPS) on the web interface of Firefly-III
Panel. Set it `true` to enable it, `false` otherwise.

### Option: `certfile`

The certificate file to use for SSL.

**Note**: _The file MUST be stored in `/ssl/`, which is the default._

### Option: `keyfile`

The private key file to use for SSL.

**Note**: _The file MUST be stored in `/ssl/`, which is the default._

### Option: `remote_mysql_host`

If using an external database, the hostname/address for the MYSQL/MariaDB
database.

### Option: `remote_mysql_database`

Only applies if a remote MYSQL database is used, the name of the database.

### Option: `remote_mysql_username`

Only applies if a remote MYSQL database is used, the username with permissions.

### Option: `remote_mysql_password`

Only applies if a remote MYSQL database is used, the password of the above user.

### Option: `remote_mysql_port`

Only applies if a remote MYSQL database is used, the port that the database
server is listening on.

### Option: `mapbox_api_key`

Your Mapbox API key for showing a map on the page of a tag.

### Option: `app_url`

Set APP_URL to the URL Firefly III will be on. For example `https://firefly.example.com`.

### Option: `trusted_proxy`

Only applies when using a reverse proxy. Set it to `**` and
reverse proxies work just fine.

## Database usage

By default, Firefly-III will automatically use and configure the Home Assistant
MariaDB addon which should be installed prior to startup, this can be changed
within the configuration to use an external MySql/MariaDB Database. Please note
that there is no easy upgrade path between the two options.

## Known issues and limitations

- SMTP support is disabled.
- Ingress is not supported.

## Changelog & Releases

This repository keeps a change log using [GitHub's releases][releases]
functionality. The format of the log is based on
[Keep a Changelog][keepchangelog].

Releases are based on [Semantic Versioning][semver], and use the format
of `MAJOR.MINOR.PATCH`. In a nutshell, the version will be incremented
based on the following:

- `MAJOR`: Incompatible or major changes.
- `MINOR`: Backwards-compatible new features and enhancements.
- `PATCH`: Backwards-compatible bugfixes and package updates.

## Support

Got questions?

You have several options to get them answered:

- The [Home Assistant Community Add-ons Discord chat server][discord] for add-on
  support and feature requests.
- The [Home Assistant Discord chat server][discord-ha] for general Home
  Assistant discussions and questions.
- The Home Assistant [Community Forum][forum].
- Join the [Reddit subreddit][reddit] in [/r/homeassistant][reddit]

You could also [open an issue here][issue] GitHub.

## Authors & contributors

The original setup of this repository is by [Paul Sinclair][sinclairpaul]. The repository was later forked by Paulo Costa after the initial author made its repo read-only.

For a full list of past authors and contributors, check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2020-2023 Paulo Costa

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[firefly-iii]: https://firefly-iii.org/
[contributors]: https://github.com/coostax/addon-firefly-iii/graphs/contributors
[discord-ha]: https://discord.gg/c5DvZ4e
[discord]: https://discord.me/hassioaddons
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg
[forum]: https://community.home-assistant.io/?u=frenck
[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
[release-shield]: https://img.shields.io/badge/version-v3.1.18-blue.svg
[release]: https://github.com/coostax/addon-firefly-iii/tree/v3.1.18