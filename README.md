# Cosmology Updates

## 2023-10-30 ~ 2023-11-03 Week 26
1. [30%] Rebuild NFT example with Interchain UI
   * Upgrade @cosmos-kit/* deps in nft and nft-new example
   * Update common and wallet components
   * Other small refactorings

## 2023-10-23 ~ 2023-10-27 Week 25
1. [Done Finally] Rebuild swap-tokens example with Interchain UI
   * Review needed from Luca
   * [PR] https://github.com/cosmology-tech/create-cosmos-app/pull/139
   * The original folder was renamed to `swap-tokens-chakra` (Should we keep this folder?)
2. [10%] Start working on the NFT example with Interchain UI
     
## 2023-10-09 ~ 2023-10-20 Week 23~24
1. [80% Done] Refactor/Rebuild Swap Component with Interchain UI
   * Swap.tsx
   * SwapButton.tsx
   * SwapFromTo.tsx
   * SwapInfo.tsx
   * SwapPrice.tsx
   * SwapResult.tsx
   * SwapRoute.tsx
   * SwapSlippage.tsx
   * SwapTokenInput.tsx
2. Refactor hooks in Swap Tokens example
   * useSwap
   * usePools
   * usePrices
   * useBalances
3. [Code] https://github.com/cosmology-tech/create-cosmos-app/compare/swap-tokens-new?expand=1
4. [Not Started] Account Abstraction Support https://github.com/burnt-labs/cosmos-kit/pull/2/files#diff-211385fbb4310c997955e08d2e81a7ff78c8afc7d8bb1400f44c4a03c60795bdR135     

## 2023-10-02 ~ 2022-10-06 Week 22 (Holiday)

## 2023-09-25 ~ 2023-09-28 Week 21
1. [Solved] Wallet gets disconnected when switching chains https://github.com/cosmology-tech/cosmos-kit/issues/332
   * From @vinodhum from Discord
   * Wrong use of hook instead of bug after reading the code sample they provided.
   * [Suggestion] We should always ask them to create an issue and provide reproduce steps on GitHub.
2. [WIP 70%] Port swap-token example in cca to interchain-ui
   * More work to be done on the SwapToken component in interchain-ui to make is usable in examples
3. Loom
   * https://www.loom.com/share/5ef9c5083a454a018a1ebb2db1db91f3

## 2023-09-18 ~ 2023-09-22 Week 20
1. [WIP 60%] Port swap-token example in cca to interchain-ui
   * [Done] Rebuild the wallet compoment(s) with interchain-ui (`70%` less code)
   * [Code] https://github.com/cosmology-tech/create-cosmos-app/commit/edb00943fb17b7de8fb2e5d804f0937af980da65#diff-e4688342543e6e8a849f65ac5f3e7768cb7aeb86ce7ae8e4c9aec40e8862e8dd
  
   | Component Name | LOC | New Component Name | LOC |
   |----------------|-----|--------------------|-----|
   | AddressCard    | 206 | ClipboardCopyText  |  1  |
   | ChainCard      |  44 |          Chain     |  44 |
   | UserInfo       |  36 |           User     |  20 |
   | Wallet         | 151 |        Wallet      |  65 |
   | WalletConnect  | 210 |        Connect     |  60 |
   | WarnBlock      |  90 |        Warning     |  33 |
   | All            | 737 |           All      | 223 |

   * [WIP] Replace the swap component with SwapToken component in interchain-ui
   * Loom
   https://www.loom.com/share/2f8b8111f54743959f1c57d24ab6092a  
   
## 2023-09-11 ~ 2023-09-15 Week 19
1. [Merged & Done] Flip logos for MetaMask Snaps
   <img width="313" alt="image" src="https://github.com/cosmology-tech/cosmos-kit/assets/7459812/932b8d6b-4423-4612-ac1a-ecb5ac46ca26">
   * PR1 https://github.com/cosmology-tech/cosmos-kit/pull/322
   * PR2 https://github.com/cosmology-tech/interchain-ui/pull/102
2. [Merged & Done] Add docs for MetaMask Snaps
   * PR https://github.com/cosmology-tech/cosmos-kit/pull/326
3. [WIP] Port `swap-token` example in cca to `interchain-ui`
4. Loom
   * https://www.loom.com/share/bef87948ddc44cf681a358bcb37ce81a

## 2023-09-04 ~ 2023-09-08 Week 18
1. metamask snap support https://github.com/cosmology-tech/cosmos-kit/issues/301
   * Funtionality has been done
   * Field name to indicate an MetaMask Snap
     - Currently `metamask_snap: true` is used https://github.com/cosmology-tech/cosmos-kit/issues/302
     - For scalibility, consider using `extends` field whose value can be 'MetaMask' or some other wallet names in the future
     - `MetaMask Snaps` `Keplr Addons` `Leap Plugins`
<img width="305" alt="image" src="https://github.com/twhy/cosmology-updates/assets/7459812/6ef85c68-0282-466e-acfe-d129ca649531">
<img width="1101" alt="image" src="https://github.com/twhy/cosmology-updates/assets/7459812/226cee97-4c82-46e6-b42c-f7b61806bd57">
2. Loom
https://www.loom.com/share/b09c2cf7621249d5af9791fab18fa060

## 2023-08-28 ~ 2023-09-01 Week 17
1. [Fixed & Published] useChains bug when one chain has connected https://github.com/cosmology-tech/cosmos-kit/issues/308
   * [PR Merged] https://github.com/cosmology-tech/cosmos-kit/pull/309/files
   * [Docs] useChains nav in docs is missing
2. [WIP] Enable broadcast for Ledger
   * add `getOfflineSigner` in Ledger client class
3. Loom
   * https://www.loom.com/share/d29ee66b96484bdb8ea5f8aa8a90b0ec
   
## 2023-08-21 ~ 2023-08-25 Week 16
1. Refactor the asset-list example in cca with Interchain UI https://github.com/cosmology-tech/projects-issues/issues/408
   * Lacking components, features, and docs are blocking this work
   * Meet with Phat and Marshall with blocking items
   * [Solution] Phat make an `asset-list-app` that replace all chakra-ui with interchain-ui in `asset-list` example so that I can use it as an refenence to update the rest examples.

## 2023-08-14 ~ 2023-08-18 Week 15
1. Refactor the asset-list example in cca with Interchain UI https://github.com/cosmology-tech/projects-issues/issues/408
   * Replace Chakra UI components with Interchain UI
   * Refactor `Header.tsx` with TailwindCSS (60 lines => 34 lines)
   * Refactor `Footer.tsx` with TailwindCSS (130 lines => 50 lines)
2. Interchain UI Improvements (TBD)
   * Add `toggleTheme()` method
   * Complete `Button` component (naming and features)
3. Loom
   https://www.loom.com/share/62ef5619fccf48d6aa2b641e2f8782ff

## 2023-08-07 ~ 2023-08-11 Week 14
1. `useChains` https://github.com/cosmology-tech/cosmos-kit/issues/263
   * [Review Needed] **PR** https://github.com/cosmology-tech/cosmos-kit/pull/293
   * Docs Added
   * Work with extensions and mobile apps, no duplicate popups
2. Loom
   * https://www.loom.com/share/93da0afe688141148fd95b4cfbbf2081  
   * `useChains` Demo https://www.loom.com/share/8d44cbd1c8a8472db63a90950dcbe339
## 2023-07-31 ~ 2023-08-04 Week 13
1. (WIP) `useChains` WalletConnect part https://github.com/cosmology-tech/cosmos-kit/issues/263
   * Works with WalletConnect
   * [TODO] Fix duplicate popups on mobile apps when reconnect
   * [Code] https://github.com/cosmology-tech/cosmos-kit/compare/use-chains?expand=1
   * <img width="360" alt="image" src="https://github.com/twhy/cosmology-updates/assets/7459812/b93f1f24-206d-4d5b-bf73-787cef267a0a">
2. (WIP) Refactor the asset-list example in cca with Interchain UI https://github.com/cosmology-tech/projects-issues/issues/408
3. Loom
   * https://www.loom.com/share/4cd4e15b818c4ca988ea4ca4218976b0

## 2023-07-24 ~ 2023-07-28 Week 12
1. Add docs for new `cosmos-kit` package  
   https://github.com/cosmology-tech/cosmos-kit/blob/main/packages/docs/pages/integrating-wallets/adding-all-wallets.mdx
2. Add `useChains` hook (WIP, extension part has worked)
   * Issue https://github.com/cosmology-tech/cosmos-kit/issues/263
   * Code https://github.com/cosmology-tech/cosmos-kit/compare/use-chains?expand=1
   * <img width="360" alt="image" src="https://github.com/twhy/cosmology-updates/assets/7459812/e2cb8a96-6f3e-42cb-9cd7-32300c68db4c">
   
3. Loom
   https://www.loom.com/share/ebc0bb8523734658818c16afa89fea46

## 2023-07-17 ~ 2023-07-21 Week 11
1. [Released] The new cosmos-kit (v0.12.3) has released.
   * Changed version to v2.0.3 to match up with other packages.
   * Will release a minor version today / tomorrow
   * [TODO] Replace the wallet deps with `cosmos-kit` in `docs` and `example`
2. Attend a Cosmos meetup in Shenzhen
   * There were about `100` people at the meetup.
   * I couldn't believe there are so many people interested in/working on Cosmos related projects in China
   * Z gave a talk on our company and tools
![WechatIMG49](https://github.com/twhy/cosmology-updates/assets/7459812/777ab547-0f64-4a36-abe6-88a35032388c)
![WechatIMG47](https://github.com/twhy/cosmology-updates/assets/7459812/67b45f5e-e82b-4e80-bfbe-a1028e27e45a)
![WechatIMG48](https://github.com/twhy/cosmology-updates/assets/7459812/e64161c4-1856-4121-82cb-b3f00f8ac82f)
3. Loom
https://www.loom.com/share/35e6a7d0e67c453da083c4b6397207fd

## 2023-07-10 ~ 2023-07-14 Week 10
0. Sick for 3 days
1. Improve Ledger example page
2. Add docs on how to connect multiple chains
   ![WX20230718-120757@2x](https://github.com/twhy/cosmology-updates/assets/7459812/e5e7f568-9758-4b34-964b-8d8ad7ed7d40)
3. Loom
   https://www.loom.com/share/bd57ef501e1c4d9dacd24da50bb32070

## 2023-07-03 ~ 2023-07-07 Week 9
1. [WIP] add a new cosmos-kit package that installs the react model with EVERY wallet included https://github.com/orgs/cosmology-tech/projects/6/views/17?pane=issue&itemId=31921808
   * [Folder] I put this package at `cosmos-kit/packages/main`
   * [Code] https://github.com/cosmology-tech/cosmos-kit/compare/feat/cosmos-kit-all-wallets?expand=1
   * `wallets` Array with methods & properties & testings
   ```javascript
   import { wallets } from 'cosmos-kit'
   
   wallets.mobile      // An array of mobile wallets
   wallets.extension   // An array of extension wallets
   wallets.for('keplr', 'cosmostation')            // [KeplrExtensionWallet, KeplrMobileWallet, CosmostationExtensionWallet, CosmostationMobileWallet]
   wallets.for('keplr', 'cosmostation').mobile     // [KeplrMobileWallet, CosmostationMobileWallet]
   wallets.for('keplr', 'cosmostation').extension  // [KeplrExtensionWallet, CosmostationExtensionWallet]
   wallets.not('coin98', 'compass')                // wallets except Coin98 and Compass
   wallets.keplr           // [KeplrExtensionWallet, KeplrMobileWallet]
   wallets.keplr.mobile    // KeplrMobileWallet
   wallets.keplr.extension // KeplrExtensionWallet
   ```
   * [Question 1] What else should I add to this package ?   
      A preconfigured `ChainProvider` doesn't make sense because every Dapp has it own `walletConnectOptions`
   * [Question 2] What do you think about the package foler location `cosmos-kit/packages/main` ?
     
2. [Beta] Add a example page `ledger.tsx` in `packages/examples`
   * https://github.com/cosmology-tech/cosmos-kit/commit/51c794eb0ff305ce87bc4342d52125f67700ca7e
   * Currenty in `beta` branch
3. [Merged] Cosmostation inject script for mobile
   * Original PR https://github.com/cosmology-tech/cosmos-kit/pull/252
   * Merged PR https://github.com/cosmology-tech/cosmos-kit/pull/258
4. [Merged] Merge and publish Leap WebView support feature when it's done
   * PR https://github.com/cosmology-tech/cosmos-kit/pull/255
5. [Merged] Upgrade dependecies for templates in `create-cosmos-app`
   * PR https://github.com/cosmology-tech/create-cosmos-app/pull/118
6. Loom Videos
   * Part 1 https://www.loom.com/share/862a0e1fbb1b4cdd9e42f0f1d34ac0f3
   * Part 2 https://www.loom.com/share/8e9361ecf1ec47709b3147fcf9003c39
## 2023-06-23 ~ 2023-06-28 Week 8
1. [Closed] TypeError TS2322 'XDEFIExtensionWallet’ is not assignable to type ‘MainWalletBase' https://github.com/cosmology-tech/cosmos-kit/issues/248
   ```
   Type ‘XDEFIExtensionWallet’ is not assignable to type ‘MainWalletBase’. Property ‘_chainWalletMap’ is protected but type ‘MainWalletBase’ is not a class derived from ‘MainWalletBase’.
   ```
   * When trying to integrate XDEFI extension wallet, find this TypeError.
   * [Root Cause] XDEFI depends on `@cosmos-kit@1.7.0` and template from `cca` depends on older version of `@cosmos-kit/@react` which depends on `@cosmos-kit@core@1.3.0`
   * [Solution] Upgrade dependency versions
     ![2023-07-03 23 27 04](https://github.com/twhy/cosmology-updates/assets/7459812/94e4820e-9247-4823-98a8-6072d0a7f9d5)
   * [Improvement] Update `@cosmos-kit` related deps to lastest for templates in `cca`

2. [Merged & Done] Add related projects to every package in cosmos-kit https://github.com/orgs/cosmology-tech/projects/6/views/17?pane=issue&itemId=31921585
3. [In Review] Enable extension wallets in Leap Mobile WebView https://github.com/cosmology-tech/cosmos-kit/issues/247
   * PR https://github.com/cosmology-tech/cosmos-kit/pull/255
   * Minor issue need to tested by Leap team within their App
4. Loom video
   https://www.loom.com/share/d6d794e44ab34f66a260bd6ce46a73ba

## 2023-06-19 ~ 2023-06-21 Week 7 
1. [Closed] @cosmos-kit/react - Module not found: Can't resolve 'fs' https://github.com/cosmology-tech/cosmos-kit/issues/237
   * Can't reproduce with proejct template from `cca`
   * Works after users changed their packages version(s)
2. [Review Needed] Integrate Ledger Wallet https://github.com/cosmology-tech/cosmos-kit/issues/213
   * Pull Request https://github.com/cosmology-tech/cosmos-kit/pull/243
   * Docs Added. `@cosmos-kit/ledger` is currently in beta because
     1. This connector is a new kind of connector, and using experimental Web USB/HID APIs.
     2. Trying out the One Package Approach mentioned last week in this package. It works.
     ```typescript
     // If you want to connect to Ledger via WebUSB
     import { wallets as ledger } from '@cosmos-kit/ledger/web-usb';
 
     // If you want to connect to Ledger via WebHID
     import { wallets as ledger } from '@cosmos-kit/ledger/web-hid';

     // If later we add support for bluetooth connection
     import { wallets as ledger } from '@cosmos-kit/ledger/web-ble';
     ```
     ![WX20230627-004205](https://github.com/twhy/cosmology-updates/assets/7459812/0c70822d-b9df-4a7b-a324-81e54fffbbdd)

3. Loom https://www.loom.com/share/e16403193f114c9d82e611cb764aee8c   
## 2023-06-12 ~ 2023-06-16 Week 6
1. [90% Done] Connect to Ledger using WebUSB/WebHID
   * [Works] Connect to Ledger ✅
   * [Works] Get address and public key ✅
   * [Implemeted but not tested] Sign method
   * [Code] https://github.com/cosmology-tech/cosmos-kit/compare/feat/ledger-web-usb-hid?expand=1
   * [Issue] Describe below
  ```javascript
  // wallets/ledger/src/web-usb-hid/main-wallet.ts

  export class LedgerMainWallet extends MainWalletBase {
   // ...
   async initClient() {
    this.initingClient();
    try {
      // The line below requests USB/HID connection, but throws an error in console,
      // because requesting USB/HID connection requires a user interaction like clicking a button,
      // but there's no user interactions here. Should move this line to some method run after user clicks.
      const ledger = await getCosmosApp(this.transportType);  
      this.initClientDone(ledger ? new LedgerClient(ledger) : undefined);
    } catch (error) {
      this.logger?.error(error);
      this.initClientError(error);
    }
   }
  }
  ```
  ![WX20230621-001821@2x](https://github.com/twhy/cosmology-updates/assets/7459812/b6495f18-34b3-4e8e-bdb1-760d9bed8f32)

2. [Idea] Combining related wallet packages
  - Take Keplr for example, we got `@cosmos-kit/keplr` `@cosmos-kit/keplr-extension` `@cosmos-kit/keplr-mobile`
  - The idea is to combine these three packages into one: `@cosmos-kit/keplr`
  - Source Code Structure
  ```sh
  wallets/
    keplr/
      src/
        extension/
          ... extension code
        mobile/
          ... mobile code
        index.ts     // exporting extension and mobile wallets
      ... config files
      package.json
  ```
  - Usage
  ```typescript
  import { wallets as keplr } from '@cosmos-kit/keplr'  // extension and mobile wallets

  import { wallets as keplr } from '@cosmos-kit/keplr/extension'  // extension only

  import { wallets as keplr } from '@cosmos-kit/keplr/mobile'     // mobile only
  ```
  - Pros
    * Much Less packages.
    * More clear code structure.
    * Two third of duplicate config files can be removed from repo.
  - Cons
    * Any?

  We can discuss about this with June when she comes back.
  
* Loom Video https://www.loom.com/share/508650899aa14efdba9fb0031a0940cf

## 2023-06-05 ~ 2023-06-09 Week 5
* [Fixed & Merged] CosmosKit wallet connect error https://github.com/cosmology-tech/projects-issues/issues/349
  * Forgot to include this in the Loom video
  * PR https://github.com/cosmology-tech/cosmos-kit/pull/219
* [Done & Merged] Arbitrary signatures https://github.com/cosmology-tech/cosmos-kit/issues/89
* [Review Needed] Embed Wallet logos https://github.com/cosmology-tech/cosmos-kit/issues/230 
  - PR https://github.com/cosmology-tech/cosmos-kit/pull/229
  - [Docs Added] Only `svg` and `png` are supported. Use logo files that are less than 50kb.
  - ![WX20230613-001159@2x](https://github.com/twhy/cosmology-updates/assets/7459812/95d67425-3855-4130-baf3-8e6508c5a776)
* Loom
  - Recorded on my laptop so it's much clear now
  - https://www.loom.com/share/ab6144430435437b8a4f83b4909b8c0f
## 2023-05-29 ~ 2023-06-02 Week 4
* Integrate Ledger Wallet https://github.com/cosmology-tech/cosmos-kit/issues/213
  * Ledger Live Mobile (The WalletConnect part works, but we need Ledger team to add support to Cosmos chains)
  * Ledger Live Desktop (The WalletConnect part works, but we need Ledger team to add support to Cosmos chains)
  * Loom Video: https://www.loom.com/share/d28d7e44c56c47f2b06460c40a9ec019
  * Code changes: https://github.com/cosmology-tech/cosmos-kit/compare/ledger?expand=1
  * [Question 1] What do we usually do to "push" them to work politetly?  
    - I asked about when they will support Cosmos chains and no replys yet.
  * [Question 2] Should I try to add these features for them?   
    - Their apps are open source https://github.com/LedgerHQ/ledger-live
  
  ![WX20230604-205804@2x](https://github.com/twhy/cosmology-updates/assets/7459812/70ff4f41-c2b1-403e-8198-6b35d5caeae8)
  ![WX20230606-080445@2x](https://github.com/twhy/cosmology-updates/assets/7459812/d5f24706-78de-4c6d-a4f1-2b874d9959e6)
  
* [Bug][Fixed by June] Not detect account changed when mount https://github.com/cosmology-tech/cosmos-kit/issues/214
* [Fixed] Invalid status URL generated for seitestnet2 https://github.com/cosmology-tech/cosmos-kit/issues/195
  * [Cause] `create-cosmos-app` using an older version of `cosmos-kit`
  * [Action] Update `create-cosmos-app` to use lastest version of `cosmos-kit`
## 2023-05-22 ~ 2023-05-26 Week 3
* Integrate Ledger Wallet https://github.com/cosmology-tech/cosmos-kit/issues/213
  * Loom Video https://www.loom.com/share/c2230ba59ecc4f468bcdb7193b0defed
  * Code Changes (Draft) https://github.com/cosmology-tech/cosmos-kit/compare/ledger?expand=1
  * Question 1. How to debug Cosmos Kit Source Code?   
    -  Currently I use `docs` for debugger, please tell me a better way to do it if you know.
  * Question 2. Does the resposne from WallConnect Explorer API show that Leger Live only support Ethereum chain(s) when connecting with WalletConnect?
  ```json
  {
    "19177a98252e07ddfc9af2083ba8e07ef627cb6103467ffebb3f8f4205fd7927": {
        "id": "19177a98252e07ddfc9af2083ba8e07ef627cb6103467ffebb3f8f4205fd7927",
        "name": "Ledger Live",
        "slug": "ledger-live",
        "description": "Web3 Wallet from the company that produced the world's most secure crypto hardware device.",
        "homepage": "https://www.ledger.com/ledger-live",
        "chains": [
            "eip155:1",
            "eip155:137",
            "eip155:4",
            "eip155:56"
        ],
        "versions": [
            "1",
            "2"
        ],
        "sdks": [
            "sign_v1",
            "sign_v2"
        ],
        "app_type": "wallet",
        "image_id": "a7f416de-aa03-4c5e-3280-ab49269aef00",
        "image_url": {
            "sm": "https://explorer-api.walletconnect.com/v3/logo/sm/a7f416de-aa03-4c5e-3280-ab49269aef00?projectId=61e6745dc9a852e0ed9ba60d28212357",
            "md": "https://explorer-api.walletconnect.com/v3/logo/md/a7f416de-aa03-4c5e-3280-ab49269aef00?projectId=61e6745dc9a852e0ed9ba60d28212357",
            "lg": "https://explorer-api.walletconnect.com/v3/logo/lg/a7f416de-aa03-4c5e-3280-ab49269aef00?projectId=61e6745dc9a852e0ed9ba60d28212357"
        },
        "app": {
            "browser": "https://www.ledger.com/ledger-live/download",
            "ios": "https://itunes.apple.com/app/id1361671700",
            "android": "https://play.google.com/store/apps/details?id=com.ledger.live",
            "mac": null,
            "windows": null,
            "linux": null,
            "chrome": null,
            "firefox": null,
            "safari": null,
            "edge": null,
            "opera": null
        },
        "injected": null,
        "mobile": {
            "native": "ledgerlive://",
            "universal": ""
        },
        "desktop": {
            "native": "ledgerlive://",
            "universal": ""
        },
        "supported_standards": [],
        "metadata": {
            "shortName": "Ledger",
            "colors": {
                "primary": "#000000",
                "secondary": "#FF5300"
            }
        },
        "updatedAt": "2021-07-30T17:48:12.565+00:00"
    }
  }
  ```

## 2023-05-15 ~ 2023-05-19 Week 2
* Fix logo urls https://github.com/cosmology-tech/cosmos-kit/issues/197
* Fix TypeError when extensions are not installed https://github.com/cosmology-tech/cosmos-kit/issues/209
* Add docs for Trust and Station https://github.com/cosmology-tech/cosmos-kit/issues/198
  - PR https://github.com/cosmology-tech/cosmos-kit/pull/208  [Merged]
* Loom Video https://www.loom.com/share/dc50b6ef372c4ad29090f8caa715caf7

## 2023-05-08 ~ 2023-05-12 Week 1
* Onboarding https://github.com/cosmology-tech/onboarding
* Fix build is failing https://github.com/cosmology-tech/cosmos-kit/issues/199
