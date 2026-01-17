# Plugin Marketplace

Claude Code 用プラグインのマーケットプレイスです。

## 概要

このリポジトリは Claude Code で使用可能なプラグインを一元管理しています。

## 登録プラグイン

| プラグイン | 説明 | スキル数 |
|-----------|------|---------|
| [miyabi-ppal-plugin](https://github.com/ShunsukeHayashi/miyabi-ppal-plugin) | Course Society - オンラインコース運営 | 6 |

## 使い方

### 1. プラグインをインストール

```bash
cd ~/.claude
git clone https://github.com/ShunsukeHayashi/miyabi-ppal-plugin.git
```

### 2. Claude Code で有効化

`~/.claude/config.json` に追加:

```json
{
  "plugins": [
    "~/.claude/miyabi-ppal-plugin"
  ]
}
```

## プラグイン登録

新しいプラグインを登録したい場合は、Pull Request を送るか、`marketplace.json` に追加してください。

## ライセンス

各プラグインのライセンスはそれぞれのリポジトリを確認してください。
