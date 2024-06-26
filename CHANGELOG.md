# Change Log

All notable changes to this project will be documented in this file.

## [Version 0.3.0] - 2024-04-12

### Added

- Allows multiple generations for each combination of parameters.
- Improved metrics are displayed after inference results
- Allows inspecting past experiments without the need to download the corresponding file.
- Displays current version number to the settings interface.
- Displays the version of Ollama running on the selected server

## [Version 0.2.1] - 2024-03-24

### Added

- Supports user input for adicional parameters: `tfs_z`, `mirostat`, `mirostat_eta` and `mirostat_tau`.

## [Version 0.2.0] - 2024-03-23

### Added

- Added a "request_timeout" parameter to settings that controls the amount of time (in seconds),
  the application should wait for an inference call to complete before returning and error (for that individual call). This is useful as, IME, some combinations of parameters can make models hang.

## [Version 0.1.2] - 2024-03-14

### Added

- UI tweaks to improve prompt modal (keyboard shortcut to update + tooltip on icon)

### Changed

- Fixed issue that allowed space delimited lists to pass parameter validation.

## [Version 0.1.1] - 2024-03-14

### Added

- The textarea for the prompt can be expanded to make editing more ergonomic

### Changed

- Prevents multiple instances of the app to run simultaneously.
- Uses the [Rust path module](https://docs.rs/tauri/latest/tauri/api/path/index.html) to store experiment logs (issue #4 - Read-only file system (os error 30) on MacOS).

## [Version 0.1.0] - 2024-03-13

### Added

- Lists previous experiment logs, downloadable as JSON files.

## [Version 0.0.3] - 2024-03-01

### Changed

- Added `Total Duration` ellapsed time to results metadata.
- Calculates `Throughput` based on `total duration` instead of `eval duration`.

## [Version 0.0.2] - 2024-03-01

### Added

- You can now define a list of `repeat_last_n` parameters when running a grid-search.
- Added a changelog.

### Changed

- Added definitions of concepts to starting screen.
