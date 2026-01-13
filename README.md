# Yukioni - 雪鬼ごっこミニゲーム

> ⚠️ **α版（アルファ版）** - このプラグインは現在開発中です。機能が不完全な場合やバグが存在する可能性があります。

雪鬼ごっこをMinecraftで遊べるSpigot/Paperプラグインです。

## 概要

鬼と市民に分かれて遊ぶ鬼ごっこゲームです。鬼は雪ブロックを投げて市民を鬼に変え、市民は制限時間内に逃げ切れば勝利します。

## ⚠️ α版について

このプラグインは**アルファ版**です：
- 機能が不完全な場合があります
- バグが存在する可能性があります
- 今後のアップデートで仕様が変更される場合があります
- 問題を発見した場合は [Discord](https://discord.gg/zYY55dzhjd) でご報告ください

## ダウンロード

[Releases](https://github.com/henntekosennsi1-rgb/Yukioni/releases)から最新版をダウンロードしてください。

## 主な機能

- 2～16人対応
- 鬼は雪ブロックを投げて市民を捕まえる
- 市民は移動速度アップで逃げる
- ゲーム開始時の鬼凍結時間（10秒）
- 雪ブロック投げクールダウン
- ゲームエリア設定
- 看板での参加/退出
- アクションバーでタイマー表示

## ゲームルール

| 役職 | 説明 |
|------|------|
| **鬼** | 雪ブロックを投げて市民を鬼にする |
| **市民** | 鬼から逃げて時間切れまで生き残る |

**勝利条件**
- 鬼の勝利: 全員が鬼になる
- 市民の勝利: 時間切れまで1人以上生き残る

## コマンド

| コマンド | 説明 |
|---------|------|
| `/yukioni setup spawn` | 退出時スポーン設定 |
| `/yukioni setup lobby` | ロビー設定 |
| `/yukioni setup pos1` | ゲームエリア座標1 |
| `/yukioni setup pos2` | ゲームエリア座標2 |
| `/yukioni start` | ゲーム開始 |
| `/yukioni stop` | ゲーム強制終了 |
| `/yukioni reload` | 設定再読み込み |

## 設定
```yaml
game:
  match-duration: 420    # 試合時間（秒）
  min-players: 2         # 最小人数
  max-players: 16        # 最大人数
  oni-freeze-time: 10    # 鬼の初期凍結時間
  snowblock-cooldown: 5  # 雪ブロック投げクールダウン
  citizen-speed: 0.3     # 市民の移動速度
```

## 動作環境

- Spigot/Paper 1.21.x
- Java 17以上

## コミュニティ

**Discordサーバー:** https://discord.gg/zYY55dzhjd

バグ報告・質問・要望はDiscordでお願いします！

## ライセンス

All Rights Reserved
