# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.73-T5](https://github.com/leslieyang-amec/xAisUtility/releases/tag/v3.73-T5) - 2025-06-25

### Added

- Check the integrity of the firmware upgrade file content.

### Fixed

- Querying device data during firmware upgrade.

## [3.73-T4](https://github.com/leslieyang-amec/xAisUtility/releases/tag/v3.73-T4) - 2025-06-04

### Added

- Enhance system stability
  
## [3.73-T3](https://github.com/leslieyang-amec/xAisUtility/releases/tag/v3.73-T3) - 2025-05-28

### Added

- Supports configuring the Modbus settings for the AIS AtoN.

### Fixed

- AIS AtoN does not display the destination MMSI correctly after configuring the device.
- After disconnect, the utility does not return to the default setting.

### Changed

- Add scrollability to some pages, allowing them to display all of the widgets on the small display device.

## [3.73-T2](https://github.com/leslieyang-amec/xAisUtility/releases/tag/v3.73-T2) - 2025-05-08

### Added

- Diagnostics summary file add Tx/Rx message count.
- AIS AtoN, configure the "output of all received AIS messages" setting.

### Changed

- Add a prefix name when saving serial data to a file.
- Add a prefix name when exporting device settings to a file.
- Change the AIS AtoN configure sentence sent to the device flow.

### Fixed

- AIS AtoN, configure the lantern status setting with the wrong value.

## [3.73-T1](https://github.com/leslieyang-amec/xAisUtility/releases/tag/v3.73-T1) - 2025-04-09

### Added

- While sending commands to the device, the system will pop-up a dialog to display  sending progress and prevent user action.
- Product information setting page/tab for B620.
- New application type, configuration universal.
  Utility will detect the device type then update utility icon and toggle hide/show tabs.
- New qwLabelText widget module.
- Disable ublox NINA bluetooth command when generate commands.
- Display AtoN name on the home page.
- N323 redundant configuration
- Popup message box with auto close

### Changed

- N323 chaining list placeholder text.
- Encryption key configuration interface. Unify NMEA 0183 CEK related module.
- Device setting page, always initial the MANDO and N323 pages.
- AIS Configuration tool support both AIS Class B and AIS AtoN device.
- Migrate Qt to 6.9
- Import setting file will trigger read device setting.
- AIS AtoN configuration sentence generation order change from by station to by sentence formatter.
- Version naming rule.

### Fixed

- Set CAMINO-108 GNSS system default selection to be GPS + Glonass.
- N323 setting off-position SRM message content with wrong encoding.
- B620/B650 parser PAMC BIIT output sub ID value. 
- Firmware upgrade handle device reboot time out procedure
- Disable pop up progress bar if only send one NMEA 0183 sentence
- Firmware upgrade path prefix
- Firmware upgrade session won't re-connect when connect type is ethernet
- MacOS CMakeLitst.txt
 
### Removed

- Detect device type fail error message.
- xMsg::Send_NMEA0183_Query singal.
- 

## [3.72] - 2024-08-28

### Added

- Add long press feature to trigger some special event for touchscreen usage.

### Fixed

- For the B600 series, reset the device GNSS ROM version value after disconnecting to prevent displaying unsupported GNSS selection items. 

## [3.71] - 2024-07-31

### Added

- Support B108W (ublox NINA) and B600W (ublox NINA) model.
- GNSS NMEA version configurable feature (B600 series).
- Support display multi GNSS system information.
- Neutral design, it can provide for ODM customers to use without any extra modification.

## [X.Y.Z] - YYYY-MM-DD

- `Added` for new features.
- `Changed` for changes in existing functionality.
- `Deprecated` for soon-to-be removed features.
- `Removed` for now removed features.
- `Fixed` for any bug fixes.
- `Security` in case of vulnerabilities.

[3.71]: https://gitlab.base.alltekmarine.com/leslieyang/aisdev/-/tags/3.71
