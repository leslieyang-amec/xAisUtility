# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.73] - 2025-08-28

### Fixed
修正

- Query the AIS AtoN TAG Block setting process by an incorrect query sentence.
當詢問AIS AtoN TAG Block設定值，詢問語句錯誤

- Querying device data during firmware upgrade.
當進行韌體更新時，utility還會詢問設備設定值

- AIS AtoN does not display the destination MMSI correctly after configuring the device.
當設定AIS AtoN的destination設定後，更新後畫面不會顯示正確的數值

- After disconnect, the utility does not return to the default setting.
當disconnect之後，畫面上顯示不會變成預設值

- N323 setting off-position SRM message content with wrong encoding.
設定N323的off-position的SRM訊息內容，訊息內容設定會失敗

- Firmware upgrade session won't reconnect when the connection type is Ethernet
透過ethernet進行韌體更新，不會自動重新連線

### Changed
修改

- Display the order of configuring the GNSS system.
修改GNSS系統顯示順序

- Add a prefix name when saving serial data to a file.
修改儲存serial資料時，預設檔名

- Add a prefix name when exporting device settings to a file.
修改儲存device資料時，預設檔名

- Version naming rule.
修改軟體版本命名規則 

### Added
新增

- Configure NMEA 0183 SPO for AIS AtoN device.
設定AIS AtoN的NMEA 0183 SPO參數

- Check the integrity of the firmware upgrade file content.
檢查firmware upgrade檔案內的版本以及適用的設備

- Diagnostics summary file add Tx/Rx message count.
分析報告檔案內容包含 Tx/Rx訊息數量

- AIS AtoN, configure the "Output all Rx messages" setting.
設定 AIS AtoN 開啟或關閉輸出所有Rx AIS訊息功能

- While sending commands to the device, the system will pop-up a dialog to display sending progress and prevent user action.
當在傳送資料給設備時，會跳出視窗告知客戶，避免此時客戶繼續操作

- Display AtoN name on the home page.
顯示 AIS AtoN 名稱於首頁

- N323 redundant configuration
N323 redundant 功能設定

## [3.72] - 2024-08-28

### Added

- Add long-press feature to trigger a special event for touchscreen usage.

### Fixed

- For the B600 series, reset the device GNSS ROM version value after disconnecting to prevent displaying unsupported GNSS selection items. 

## [3.71] - 2024-07-31

### Added

- Support B108W (ublox NINA) and B600W (ublox NINA) models.
- GNSS NMEA version configurable feature (B600 series).
- Support displaying multiple GNSS system information.

## [X.Y.Z] - YYYY-MM-DD

- `Added` for new features.
- `Changed` for changes in existing functionality.
- `Deprecated` for soon-to-be removed features.
- `Removed` for now removed features.
- `Fixed` for any bug fixes.
- `Security` in case of vulnerabilities.

[3.71]: https://gitlab.base.alltekmarine.com/leslieyang/aisdev/-/tags/3.71
