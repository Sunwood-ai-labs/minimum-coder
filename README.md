<p align="center">
  <img src="./assets/header.svg" alt="Minimum Coder Header" width="800">
</p>

# 🌟 Minimum Coder

これは[Coder](https://github.com/coder/coder)の最小構成版です。リモート開発環境を簡単にセットアップし、どこからでも開発作業が行えるようにする軽量なソリューションです。

## 💡 概要

Minimum Coderは以下の機能を提供する最小限のセットアップを実現しています：

- 🔨 任意のクラウドでの開発環境構築
- 💻 主要なIDEサポート（VS Code、JetBrains等）
- 🔒 セキュアなリモートアクセス
- 🚀 高速な開発環境

## ⚙️ 動作環境

- Docker
- Docker Compose

## 📦 インストール

1. このリポジトリをクローン：
```bash
git clone https://github.com/yourusername/minimum-coder.git
cd minimum-coder
```

2. 環境の起動：
```bash
docker-compose up -d
```

## 🚀 使用方法

1. ブラウザで開発環境にアクセス：
```
http://localhost:3000
```

2. お好みのIDEを使用して開発を開始

## 🔧 設定

設定は`docker-compose.yaml`で管理されています。主な設定項目：

- ポート設定
- 開発環境の基本設定
- ストレージ設定

## 🤝 貢献

プルリクエストやイシューの報告を歓迎します。大きな変更を加える場合は、まずイシューで変更内容を議論してください。

## 📝 ライセンス

このプロジェクトは[GNU Affero General Public License v3.0](https://github.com/coder/coder/blob/main/LICENSE)の下で公開されています。

## 📚 参考リンク

- [Coder公式ドキュメント](https://coder.com/docs/coder-oss)
- [Coder GitHub](https://github.com/coder/coder)
