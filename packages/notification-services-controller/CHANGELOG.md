# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.2]

### Added

- added catch statements in NotificationServicesController to silently fail push notifications ([#4536](https://github.com/MetaMask/core/pull/4536))

- added checks to see feature announcement environments before fetching announcements ([#4530](https://github.com/MetaMask/core/pull/4530))

### Removed

- removed retries when fetching announcements and wallet notifications. Clients are to handle retries now. ([#4531](https://github.com/MetaMask/core/pull/4531))

## [0.1.1]

### Added

- export `defaultState` for `NotificationServicesController` and `NotificationServicesPushController`. ([#4441](https://github.com/MetaMask/core/pull/4441))

- export `NOTIFICATION_CHAINS_ID` which is a const-asserted version of `NOTIFICATION_CHAINS` ([#4441](https://github.com/MetaMask/core/pull/4441))

- export `NOTIFICATION_NETWORK_CURRENCY_NAME` and `NOTIFICATION_NETWORK_CURRENCY_SYMBOL`. Allows consistent currency names and symbols for supported notification services ([#4441](https://github.com/MetaMask/core/pull/4441))

- add `isPushIntegrated` as an optional env property in the `NotificationServicesController` constructor (defaults to true) ([#4441](https://github.com/MetaMask/core/pull/4441))

### Fixed

- `NotificationServicesPushController` - removed global `self` calls for mobile compatibility ([#4441](https://github.com/MetaMask/core/pull/4441))

## [0.1.0]

### Added

- Initial release

[Unreleased]: https://github.com/MetaMask/core/compare/@metamask/notification-services-controller@0.1.2...HEAD
[0.1.2]: https://github.com/MetaMask/core/compare/@metamask/notification-services-controller@0.1.1...@metamask/notification-services-controller@0.1.2
[0.1.1]: https://github.com/MetaMask/core/compare/@metamask/notification-services-controller@0.1.0...@metamask/notification-services-controller@0.1.1
[0.1.0]: https://github.com/MetaMask/core/releases/tag/@metamask/notification-services-controller@0.1.0
