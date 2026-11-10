# ConsoleSmith

ConsoleSmith connects an AI assistant such as Claude Desktop to your Microsoft 365 and Intune tenant through Microsoft Graph, so you can look up users, groups, licenses and devices in plain language, and, with a Pro license, make a small set of changes, each one after a preview and an approval step. It runs on your own computer with an app registration in your own tenant.

This repository holds the release downloads only. The software itself is in each release ZIP.

## Download

Get the current version from https://consolesmith.com/download. Older versions are on this repository's Releases page.

Each release has two files: the ZIP, for example ConsoleSmith-1.0.1.zip, and SHA256SUMS.txt. Setup instructions are in README.md inside the ZIP.

## Check the download

Before you extract the ZIP, compare its SHA-256 hash with the one in SHA256SUMS.txt and on the download page.

On Windows, in Command Prompt:

```
certutil -hashfile ConsoleSmith-1.0.1.zip SHA256
```

On macOS:

```
shasum -a 256 ConsoleSmith-1.0.1.zip
```

On Linux:

```
sha256sum ConsoleSmith-1.0.1.zip
```

If the hashes differ, do not use the file. Download it again from the link above, and write to us if it still differs.

## Supported systems

Setup is tested on Windows 11 (x64). It uses an installed 64-bit Python 3.11 to 3.14, or installs Python 3.14.10 for your user only. Windows 10 is not supported.

The ZIP also includes a setup script for Apple Silicon Macs and Linux (x64 or arm64), but we have not tested those yet. On them, install Python 3.11 to 3.14 first. The approval window the change tools rely on is Windows only, so on a Mac or Linux expect the change tools to be refused by default. Intel Macs are not supported.

The README inside the 1.0.1 ZIP still lists Windows 10; this page is current.

## Terms and support

Use of ConsoleSmith is governed by the Terms of Service at https://consolesmith.com/terms. The Privacy Policy is at https://consolesmith.com/privacy. See LICENSE and NOTICE.

Support is by email at support@consolesmith.com. Please report security issues to security@consolesmith.com.

Issues and discussions are turned off on this repository.
