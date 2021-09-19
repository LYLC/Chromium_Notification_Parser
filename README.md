## Introduction

Google Chrome, Microsoft Edge and Brave Browser are based on Chromium. When websites use Push API to send the notifications to those browsers, Chromium will store the notifications and their metadata in a LevelDB database, which can be found in the "Platform Notifcations" folder.

A LevelDB database is comprised with several files. The notification information is stored in a .log file and .ldb file (if it exists). This tool is developed to parse notifications and their metadata in the .log file.

Testings have been done before this release. Use it as is. It supports Windows, Linux and macOS. However, please feel free to reach out to me if any bugs are found.

## Version
0.1.0

## Usage
Usage: chromium_notification_parser [CHROMIUM_NOTIFICATION_LOG_FILE]

## Example
chromium_notification_parser 000003.log

## Supported Output Format
CSV

## Supported Operating Systems
* Ubuntu 20.04 x64 (tested)
* macOS Big Sur 11.6 (tested)

It may work on other Ubuntu and macOS version. However, testings are required to confirm it.

## SHA256
1c6157fb33b8d256c564ebb3e0a17536bda1b13b7139091f3469ece41e0833db  chromium_notification_parser-0.1.0-Ubuntu.zip
e926e5fb6022b13d62cad69474d8e7c21cfd0638e438e617546321e006b2078b  chromium_notification_parser-0.1.0-Windows.zip
e87358253a9b30aaaaeef333d74568067f4282390a5690f94fc8537a13bb995b  chromium_notification_parser-0.1.0-macOS.zip

## Notes
* The date format is yyyy-mm-dd.
