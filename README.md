# Home Assistant Add-ons

![Project Stage][project-stage-shield]
![Maintenance][maintenance-shield]
[![License][license-shield]](LICENSE.md)

## About

Home Assistant allows anyone to create add-on repositories to share their
add-ons for Home Assistant easily. This repository is one of those repositories,
providing extra Home Assistant add-ons for your installation.

## Installation

Adding this add-ons repository to your Home Assistant instance is pretty easy. In the
Home Assistant add-on store, click on the three dots at the top right corner,
select repositories and on the Add line paste the following URL to add this repository:

```txt
https://github.com/coostax/ha-addons
```

## Add-ons provided by this repository

### &#10003; [Firefly III][addon-firefly-iii]

![Latest Version][firefly-iii-version-shield]
![Supports armhf Architecture][firefly-iii-armhf-shield]
![Supports armv7 Architecture][firefly-iii-armv7-shield]
![Supports aarch64 Architecture][firefly-iii-aarch64-shield]
![Supports amd64 Architecture][firefly-iii-amd64-shield]
![Supports i386 Architecture][firefly-iii-i386-shield]

A free and open source personal finance manager

[:books: Firefly III add-on documentation][addon-doc-firefly-iii]

### &#10003; [Wallabag][addon-wallabag]

![Latest Version][wallabag-version-shield]
![Supports armhf Architecture][wallabag-armhf-shield]
![Supports armv7 Architecture][wallabag-armv7-shield]
![Supports aarch64 Architecture][wallabag-aarch64-shield]
![Supports amd64 Architecture][wallabag-amd64-shield]
![Supports i386 Architecture][wallabag-i386-shield]

A web application allowing you to save web pages for later reading

[:books: Wallabag add-on documentation][addon-doc-wallabag]

## Releases

Releases are based on [Semantic Versioning][semver], and use the format
of ``MAJOR.MINOR.PATCH``. In a nutshell, the version will be incremented
based on the following:

- ``MAJOR``: Incompatible or major changes.
- ``MINOR``: Backwards-compatible new features and enhancements.
- ``PATCH``: Backwards-compatible bugfixes and package updates.

## License

MIT License

Copyright (c) 2022 Paulo Costa

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


[addon-firefly-iii]: https://github.com/coostax/addon-firefly-iii/tree/v3.1.12
[addon-doc-firefly-iii]: https://github.com/coostax/addon-firefly-iii/blob/v3.1.12/README.md
[firefly-iii-issue]: https://github.com/coostax/addon-firefly-iii/issues
[firefly-iii-version-shield]: https://img.shields.io/badge/version-v3.1.12-blue.svg
[firefly-iii-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[firefly-iii-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[firefly-iii-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[firefly-iii-armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[firefly-iii-i386-shield]: https://img.shields.io/badge/i386-yes-green.svg
[addon-wallabag]: https://github.com/coostax/addon-wallabag/tree/v0.2.6
[addon-doc-wallabag]: https://github.com/coostax/addon-wallabag/blob/v0.2.6/README.md
[wallabag-issue]: https://github.com/coostax/addon-wallabag/issues
[wallabag-version-shield]: https://img.shields.io/badge/version-v0.2.6-blue.svg
[wallabag-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[wallabag-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[wallabag-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[wallabag-armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[wallabag-i386-shield]: https://img.shields.io/badge/i386-yes-green.svg

[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
[license-shield]: https://img.shields.io/github/license/coostax/coostax/ha-addons.svg
[semver]: http://semver.org/spec/v2.0.0.html