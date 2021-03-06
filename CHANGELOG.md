# Changelog

## [Upcoming]

## [Known Issues]

## [0.1.32] - 2022-07-17
### Changed
- PHPCS from 3.7.0 to 3.7.1.

### Fixed
- determining of custom lint standard if file does not exist.

## [0.1.31] - 2022-04-21
### Changed
- PHPCS from 3.6.2 to 3.7.0.

## [0.1.30] - 2022-04-21
### Fixed
- syntax error (typo).

## [0.1.29] - 2022-04-21
### Updated
- bundled PHPCS to 3.6.2 from 3.6.0.

## [0.1.28] - 2021-04-15
### Fixed
- syntax error (typo).

## [0.1.27] - 2021-04-14
### Fixed
- incorrect access when there was no linter STDIN reader available.

## [0.1.26] - 2021-04-13
### Updated
- bundled PHPCS to from 3.5.8 to 3.6.0.

## [0.1.25] - 2021-04-13
### Fixed
- a typo when using bundled PHPCS executable.

## [0.1.24] - 2021-04-13
### Fixed
- detection of project or globally configured PHPCS executable paths.

## [0.1.23] - 2021-04-08
### Fixed
- error when opening a project.

## [0.1.22] - 2021-04-07
### Fixed
- parsing of PHPCS error output.

## [0.1.21] - 2021-04-07
### Added
- configurable executable path back in.
- PHPCS version to debug output.
- PHPCS installed standards to debug output.

### Fixed
- conjoining of multiple files being linted at the same time, which caused errors.

## [0.1.20] - 2021-04-06
### Updated
- output processing to not cause all issue matching extension to fail if PHPCS
  encountered an error.

## [0.1.19] - 2021-04-06
### Fixed
- output processing to not cause all issue matching extension to fail if PHPCS
  encountered an error.

## [0.1.18] - 2021-04-04
### Fixed
- false linting errors due to "non-quiet" linter output. Reduced the verbosity
  to only provide JSON output.

## [0.1.17] - 2021-04-04
### Fixed
- handling of linter error output to not falsely trigger if the work error is
  randomly contained in the linter output.

## [0.1.16] - 2021-04-04
### Added
- catching of errors thrown by the linter. These would previously wreck the
  extension, and are now output to Nova's Extension Console.

## [0.1.15] - 2021-04-04
### Fixed
- issue with multiple processes trying to start up.

## [0.1.14] - 2021-04-04
### Added
- license details.

### Updated
- linting process to use `stdin` instead of relying on a file, which greatly
  improves performance.

## [0.1.10 to 0.1.13] - 2021-04-03
### Fixed
- license reference.

## [0.1.10] - 2021-04-03
### Added
- linter process cancelation, for the event that a new linter was started before
  the previous one finished.
- temporary file storage to lint in-buffer documents.
- configuration option to show debug logs (and conversely hide debug logs if not
  enabled).
- improved logging with more details.

## [0.1.9] - 2021-04-03
### Added
- Upcoming and Known Issues details.

## [0.1.8] - 2021-04-03
### Fixed
- implementation of additional linting information.

## [0.1.7] - 2021-04-03
### Added
- additional linting information in the message.

### Fixed
- linting hints to underling the affected word, not just the first character.

## [0.1.6] - 2021-03-31
### Removed
- elaborate extension activation processes to avoid issues for now.

## [0.1.5] - 2021-03-28
### Fixed
- self-updating of Phive binary.

## [0.1.4] - 2021-03-28
### Added
- process to update PHIVE binary.
- GPG2 binary for Phive.

## [0.1.3] - 2021-03-28
### Added
- process to set PHIVE binary chmod flags.

## [0.1.2] - 2021-03-28
### Added
- process to set PHPCS binary chmod flags.

## [0.1.1] - 2021-03-28
### Added
- PHPCS standard configuration functionality.
- PHPCS binary update when extension is loaded.

## [0.1.0] - 2021-03-28
### Added
- initial functionality.
