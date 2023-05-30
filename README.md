# Cosmology Updates

## 2023-05-08 ~ 2023-05-12 Week 1
* Onboarding https://github.com/cosmology-tech/onboarding
* Fix build is failing https://github.com/cosmology-tech/cosmos-kit/issues/199

## 2023-05-15 ~ 2023-05-19 Week 2
* Fix logo urls https://github.com/cosmology-tech/cosmos-kit/issues/197
* Fix TypeError when extensions are not installed https://github.com/cosmology-tech/cosmos-kit/issues/209
* Add docs for Trust and Station https://github.com/cosmology-tech/cosmos-kit/issues/198
  - PR https://github.com/cosmology-tech/cosmos-kit/pull/208  [Merged]
* https://www.loom.com/share/dc50b6ef372c4ad29090f8caa715caf7

## 2023-05-22 ~ 2023-05-26 Week 3
* Integrate Ledger Wallet https://github.com/cosmology-tech/cosmos-kit/issues/213
  * Question 1. How to debug Cosmos Kit Source Code?   
      Currently I use `docs` for debugger, please tell me a better way to do it if you know.
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
