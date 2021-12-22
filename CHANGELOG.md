# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Parameter to pass custom options to rsync
- Exclude .git, README.md and LICENSE by default from rsync
- Added parameter to add extra excludes to rsync (see rsync --help or man rsync)

## [1.0.0] - 2021-12-21

Initial release.

### Added

- Sync dotfiles from a git repo to a users home directory.
