# Mod Server 26.3 の MOD 配布

Minecraft 26.3 / NeoForge 26.3.0.101 のマルチサーバー用。
一度設定すると、ゲームを起動するたびに MOD が自動で最新になる。

## 最初に1回だけ（遊ぶ人）

1. **Prism Launcher** を入れる（https://prismlauncher.org/ ）。Microsoft アカウントでログイン。
2. 「インスタンスを追加」→ Minecraft **26.3** を選び、Mod ローダーで **NeoForge 26.3.0.101** を選んで作る。
3. **packwiz-installer-bootstrap.jar** をダウンロードする
   （https://github.com/packwiz/packwiz-installer-bootstrap/releases の最新版）。
4. インスタンスを右クリック →「フォルダーを開く」→ `minecraft` フォルダ（無ければ `.minecraft`）に、3 の jar を置く。
5. インスタンスの「編集」→「設定」→「カスタムコマンド」にチェックを入れ、**起動前コマンド**に次の1行を貼る。

```
"$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://nayanaoki.github.io/mc-multi-pack/pack.toml
```

6. 起動する。最初に MOD の更新画面が出て、16個が入る。そのあとサーバーに接続する。

## 2回目から

何もしなくてよい。起動するたびに、新しくなった MOD を取ってきて、外した MOD は消す。
