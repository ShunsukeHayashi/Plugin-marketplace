# Plugin Marketplace

Claude Code 用プラグインのマーケットプレイスです。

## 概要

Hayashi が開発した Claude Code プラグインを一元管理しています。

## 登録プラグイン

| プラグイン | 説明 | カテゴリ | コマンド/エージェント |
|-----------|------|---------|-------------------|
| [miyabi-ppal-plugin](https://github.com/ShunsukeHayashi/miyabi-ppal-plugin) | Course Society - オンラインコース運営 | Productivity | 6エージェント |
| [miyabi-operations](https://github.com/ShunsukeHayashi/Miyabi) | 自律型開発フレームワーク - Issue to Deploy自動化 | Development | 8コマンド/6エージェント |

## miyabi-operations

超初心者でも使える自律型開発フレームワーク。

### スラッシュコマンド

| コマンド | 説明 |
|---------|------|
| `/verify` | システム検証（環境、ビルド、テスト） |
| `/agent-run` | GitHub Issues で自律エージェント実行 |
| `/deploy` | Firebase/Cloud へデプロイ |
| `/miyabi-auto` | 完全自律パイプライン実行 |
| `/miyabi-status` | システム・エージェント状態確認 |
| `/miyabi-todos` | TODOコメント抽出・Issue作成 |
| `/security-scan` | セキュリティ脆弱性スキャン |
| `/generate-docs` | ドキュメント生成 |

### 自律エージェント

- **CoordinatorAgent** - タスクオーケストレーション
- **CodeGenAgent** - AIコード生成
- **ReviewAgent** - コード品質評価
- **IssueAgent** - Issue分析・ラベル管理
- **PRAgent** - PR自動化
- **DeploymentAgent** - CI/CD自動化

## miyabi-ppal-plugin

オンラインコース運営のための6つの専門エージェント。

### Course Society エージェント

| エージェント | 役割 |
|------------|------|
| しきるん | 統括・調整 |
| まなぶん | カリキュラム・Teachable |
| つくるん | コンテンツ制作 |
| ひろめるん | マーケティング・L-Step |
| ささえるん | サポート |
| かぞえるん | 分析・KPI |

## 使い方

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
