# lecture-to-notes

講義動画・音声・板書から、動画を見直さずに内容を理解できる日本語の学習ノートを作るためのCodexスキルです。

自分の大学の勉強用に作り、説明の詳しさや書き方を自分向けに調整しています。使うときは、理解度や好みに合わせて変更してください。

## 特徴

- 動画の時刻や「授業で省略された」といった説明に依存しない本文。
- 高校数学を前提とした簡潔な説明と、専門内容の定義・適用条件・必要な途中式。
- 体言止めの目次・見出し。
- 公式を思い出さないと議論を追いにくい箇所だけの公式参照。

このスキルはAIへの作業指示です。音声認識ソフト、モデル、HTML生成プログラム、講義資料は同梱していません。処理に使うツールは利用先の環境で確認・準備します。説明の詳しさは依頼時に変更できます。

## Codexへの導入

### GitHubから

このリポジトリのURLをCodexへ渡し、次のように依頼します。

> $skill-installer https://github.com/pealsha/lecture-to-notes の skills/lecture-to-notes をインストールして

### ZIPから

ZIPを展開し、中の `skills/lecture-to-notes` フォルダを、ユーザーのホームフォルダにある `.agents/skills/` へコピーします。

- Windows：`%USERPROFILE%\.agents\skills\lecture-to-notes\SKILL.md`
- macOS/Linux：`~/.agents/skills/lecture-to-notes/SKILL.md`

`%USERPROFILE%` と `~` は自分のホームフォルダを表します。同名のスキルがある場合は内容を確認してから更新してください。認識されない場合はCodexを再起動します。

## 利用例

> $lecture-to-notes この講義動画から、動画を見直さずに理解できる学習ノートを作って。高校数学の説明は短く、大学数学の定義・条件・必要な途中式は残して。MarkdownとローカルHTMLで保存して。

動画のファイルや保存先も一緒に指定してください。ホバー表示の動作にはHTMLなど対応する出力形式が必要です。

## 参考

[OpenAI公式：スキルの作成・配置・導入](https://learn.chatgpt.com/docs/build-skills)。友人間の手動導入にはこのフォルダを使えます。インストール可能な製品として広く配布する場合、公式はプラグイン化を推奨しています。
