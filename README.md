# Plugin Marketplace

Claude Code 用プラグインのマーケットプレイスです。

## 概要

Hayashi が開発した Claude Code プラグインを一元管理しています。

## 登録プラグイン

| プラグイン | 説明 | スキル数 |
|-----------|------|---------|
| [miyabi-ppal-plugin](https://github.com/ShunsukeHayashi/miyabi-ppal-plugin) | Course Society - オンラインコース運営 | 6 |

## 使い方

このマーケットプレイスを Claude Code に追加すると、登録済みプラグインをインストールできます。

### マーケットプレイスの追加

`~/.claude/plugins/known_marketplaces.json` に以下を追加:

```json
{
  "plugin-marketplace": {
    "source": {
      "source": "github",
      "repo": "ShunsukeHayashi/Plugin-marketplace"
    }
  }
}
```

## ライセンス

各プラグインのライセンスはそれぞれのリポジトリを確認してください。
