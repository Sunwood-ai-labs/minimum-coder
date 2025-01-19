# 🐳 Docker Template

このテンプレートは、Dockerを使用してCoderワークスペースを構築するための基本設定を提供します。

## 📋 機能

- 🔧 自動化されたワークスペースのセットアップ
- 🛠️ 事前インストールされたVS Code拡張機能
  - Python
  - Go
  - Prettier
  - ESLint
  - Terraform
  - YAML
  - Roo Cline
  - Docker
- 📊 リアルタイムリソースモニタリング
  - CPU使用率
  - メモリ使用率
  - ディスク使用量
  - ホストマシンのメトリクス

## ⚙️ 環境変数

| 変数名 | 説明 | デフォルト値 |
|--------|------|------------|
| `docker_socket` | DockerソケットのURI | `""` |

## 🚀 使用方法

1. テンプレートの選択
```bash
coder templates create docker --directory templates/docker
```

2. ワークスペースの作成
```bash
coder create --template docker my-workspace
```

## 📝 カスタマイズ

### 拡張機能の追加
`main.tf`の`startup_script`セクションで、以下のように拡張機能を追加できます：

```hcl
/tmp/code-server/bin/code-server --install-extension <extension-id>
```

### 環境変数の追加
`coder_agent.main`リソースの`env`ブロックに環境変数を追加できます：

```hcl
env = {
  MY_VAR = "value"
}
```

## 🔍 トラブルシューティング

### ワークスペースが起動しない場合
1. Dockerデーモンが実行中か確認
2. `docker ps`でコンテナの状態を確認
3. ログを確認：`coder logs my-workspace`
