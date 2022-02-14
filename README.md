# create-novel

## 使いかた

```
create-novel [title]
```

## ディレクトリ構成

![ディレクトリ構成](/image.png)

### design/
- idea.md : アイデアに関するマインドマップを行うマークダウンファイル
- character.md : キャラクター設定を行うマークダウンファイル
- worldview.md : 世界観設定を行うマークダウンファイル
- references.md : 参考文献(URL)を記述するマークダウンファイル

### summary/
- outline.txt : 文庫大賞等に応募する際に必要になるあらすじを記述するテキストファイル
- keypoint.md : 各章の概要を記述するマークダウンファイル

### draft/
- chapter*/ : 各章毎にディレクトリを分けて本編を記述するテキストファイル

### publish/
- title.txt : draft/をコンパイルすると作成されるテキストファイル(完成版)

### これは何？
たまに文庫大賞に応募する時にエディターが気分で変わっていたのでこの際VSCodeで執筆作業が完結するようにした  
これは作品毎に作成するディレクトリ構成を自動で作成するだけの自作コマンド  
基本的に執筆作業の流れは次のようになる

1. リポジトリ作成(文庫大賞投稿作品はprivate)
1. idea.mdでアイデアのマインドマップを行う
1. アイデアが固まったらcharacter.md、worldview.mdを行き来して設定資料を固める
1. keypoint.mdに小節の振り分け、各節の概要を記述していく
1. 文庫大賞用のあらすじを作成する(大抵40文字16行5ページ)
1. draft/以下に各章のディレクトリを作成、節毎にテキストファイルを作成して執筆する
1. 完成したらnovel-writerでコンパイルしてpublish/title.txtを作成して推敲する

### 執筆環境
- VSCode
  - Markmap
  - textlint
  - novel-writer
