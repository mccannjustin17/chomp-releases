# Security

Chomp opens files from anywhere and can install its own updates, so security reports are taken seriously.

## Reporting a vulnerability

Please **don't open a public issue** for security problems. Instead, report them privately through GitHub: go to the **Security** tab of this repository and choose **Report a vulnerability**.

Include what you found, the steps to reproduce it (a sample file helps, as long as it holds no private data), the Chomp version (**Chomp › About Chomp**) and your macOS version. You'll get a reply as soon as possible, and fixes ship through the built-in updater.

## How Chomp protects you

- Releases are signed with Chomp's Developer ID, use Apple's hardened runtime, and are notarized by Apple.
- Updates are only installed after the download matches its published SHA-256 checksum **and** carries a valid signature from Chomp's own developer team. Anything else is rejected and nothing is installed.
- Update checks and downloads use HTTPS and go only to GitHub, and you can turn automatic checks off in Settings.
- Your files never leave your Mac. There is no analytics or tracking.
- Saving writes a complete new file first and then swaps it into place, so a crash or full disk never leaves a half-written file.
