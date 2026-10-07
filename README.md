# blanche-de-noel-ios
クリスマスまでの 10 日間をいい子に過ごして、サンタクロースから豪華なプレゼントをもらうアドベンチャーゲーム

Unity で作ったゲーム（[blanche-de-noel-unity](https://github.com/shilokuma-inc/blanche-de-noel-unity)）を iOS 向けに書き出した Xcode プロジェクトです。

<a href="https://apps.apple.com/jp/app/blanche-de-noel/id6502287377"><img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" alt="Download Blanche de Noel on the App Store" width="120"></a>

## Environment
- Unity 2021.3.19f1
- Xcode（GitHub Actions では latest-stable）
- iOS 11.0+

## Status

| branch \ workflow | Build | Archive | Release |
| --- | --- | --- | --- |
| main | [![Build/main](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/build-main.yml/badge.svg)](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/build-main.yml) | [![Archive/main](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/archive-main.yml/badge.svg)](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/archive-main.yml) | [![Release/main](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/release-main.yml/badge.svg)](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/release-main.yml) |
| develop | [![Build/develop](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/build-develop.yml/badge.svg)](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/build-develop.yml) | [![Archive/develop](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/archive-develop.yml/badge.svg)](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/archive-develop.yml) | [![Release/develop](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/release-develop.yml/badge.svg)](https://github.com/shilokuma-inc/blanche-de-noel-ios/actions/workflows/release-develop.yml) |

| workflow | 実行トリガー | 内容 |
| --- | --- | --- |
| Build | すべてのブランチへの push | 署名なしで実機向けにビルドする |
| Archive | すべてのブランチへの push | Archive して IPA を書き出す |
| Release | `develop` / `main` への push | Archive した IPA を App Store Connect（TestFlight）へアップロードする |

## 注意
Unity から Xcode プロジェクトを書き出し直したときに、この README が消えたことがあります。書き出し後は差分を確認してから commit してください。
