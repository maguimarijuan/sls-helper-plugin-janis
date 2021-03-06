# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [2.3.0] - 2020-02-19
### Added
- `timeout` support for all API hooks
- `functionRawProps` support for all API hooks
- `eventRawProps` support for all API hooks

## [2.2.0] - 2020-02-18
### Added
- Custom authorizer support added in event listeners
- Custom authorizers can now be defined in `custom.authorizers` object in initial config and they will be remain untouched

### Fixed
- Authorizers now use the correct ARN

## [2.1.0] - 2020-02-14
### Added
- Access denied API Gateway response resource added with CORS headers

## [2.0.0] - 2020-02-10
### Added
- `authorizers` now have require the Account ID as a configuration option
- Added the `@janiscommerce/serverless-plugin-remove-authorizer-permissions` serverless plugin to allow cross-account deployments

## [1.3.4] - 2020-02-05
### Fixed
- `authorizers` now have the name property to avoid collisions

## [1.3.3] - 2020-01-22
### Fixed
- `eventListener` hook function name now includes the service name

## [1.3.2] - 2020-01-22
### Fixed
- `base` hook prune plugin typo fix

## [1.3.1] - 2020-01-21
### Fixed
- `eventListener` documentation fixed

## [1.3.0] - 2020-01-16
### Added
- `janis.api` hook added to implement custom APIs

### Changed
- Option `serviceName` changed to `serviceCode` in `janis.base` hook **BREAKING CHANGE**
- Added service name to naming, file path and API path in `janis.eventListener` hook

## [1.2.4] - 2019-12-27
### Fixed
- Authorizers in event listeners are now correctly configured

## [1.2.3] - 2019-12-27
### Fixed
- Authorizers fixed to match the correct function name

## [1.2.2] - 2019-12-26
### Fixed
- Serverless offline cache invalidation regex fixed

## [1.2.1] - 2019-12-26
### Fixed
- Service name in lower case is now in *kebab-case*

## [1.2.0] - 2019-12-26
### Added
- `apiSecrets` configuration in base hook
- Sample service example in README

### Fixed
- `base` documentation updated with required fields

## [1.1.0] - 2019-12-25
### Changed
- Runtime upgraded to nodejs.12x
- Base hook updated to the last configurations
- New authorizers added
- Event listener hook added
