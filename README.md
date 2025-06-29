# カクヨム用Slackボット

ClaudeCodeベースで動く、カクヨムの情報を探索できるSlackボット。MCPサーバーを使ってカクヨムと連携し、作品情報やランキングなどを取得する。

## 構成

- [**claude-code-slack-agent**](https://github.com/106-/claude-code-slack-agent/): Claude Codeを使ったSlackボット
- [**kakuyomu-mcp**](https://github.com/106-/kakuyomu-mcp): カクヨムAPIのMCPサーバー

## セットアップ

### 1. 設定ファイルの準備

```bash
cp config.example.yaml config.yaml
```

`config.yaml`を編集して以下の値を設定：

- `slack.signing_secret`: SlackアプリのSigning Secret
- `slack.app_token`: SlackアプリのApp Token
- `slack.bot_token`: SlackボットのBot Token  
- `claude_code.api_key`: AnthropicのAPI Key
