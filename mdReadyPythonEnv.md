---
html:
  embed_local_images: true
  embed_svg: true
  offline: true
  toc: true
export_on_save:
  html: true
---

# template markdown

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [template markdown](#template-markdown)
  - [凡例](#凡例)
  - [章立て](#章立て)
  - [pythonインストール](#pythonインストール)
    - [Pythonのバージョンについて](#pythonのバージョンについて)
      - [項](#項)
  - [画像](#画像)
    - [画像2](#画像2)
    - [画像3](#画像3)
    - [PlantUML](#plantuml)

<!-- /code_chunk_output -->

## 凡例

本書内での記述例を示す。

:::tip
知っておくと便利な小技系
:::

:::info
知っておいた方がよさそうな情報
:::

:::note
おまけ的なメモ・自分語り
:::

:::warning
極めてリスクの高い事例
:::

:::caution
注意深く利用する必要のある事例
:::

:::sample
コマンドやコードのサンプル等
:::

## 章立て

pythonインストール
  バージョンの話
  CS+は2系

VSCodeインストール

VSCodeの拡張機能インストール
  python debuggerを利用すること

  VSIXからとってくることもできるが、スペルミスには要注意  
  基本的に許可リストにあるライブラリのみ利用すること  

単純なスクリプトを実行して、挙動確認

パッケージ管理・Pythonバージョンについて

uv/pipenv環境について

JupyterNotebook環境の作成
  ライブラリの注意点
  PyPIからとってくることもできるが、スペルミスには要注意  
  基本的に許可リストにあるライブラリのみ利用すること  

セルで実行

markdownによる文書を作成したい場合は、この環境を利用する。  

- 推奨事項に追加してある拡張機能を有効化すること。
- 上記有効化してあれば、目次も自動更新される。

## pythonインストール

まずはPythonをインストールする。  

### Pythonのバージョンについて

Pythonには大まかに2.n系と3.n系が存在する。  
それぞれの主な特徴は下図の通り。  

![drawio](./img/01Python/01.drawio.png)

どちらを利用することもありうるが、本書では最新のPython環境を利用する。  

:::info
Pythonには派生形が多数存在する。  
・Circuit Python  
・Micro Python  
・Iron Python  
これらと区別するために標準のPythonをCPythonと呼称することもある。
:::

:::note
筆者が現在利用しているメイン機では2.7, 3.7～3.11をインストールしている。  
このため、利用するバージョンを使い分ける手段が必要になる。  
バージョンを使い分ける手段は後述する。  
:::

#### 項

## 画像

![画像jpg](./img/AdobeStock_489911657.jpeg){.image_w300}

### 画像2

![画像png](./img/AdobeStock_491863380.png)

pngとjpgが張り付けられることは確認した。

### 画像3

複数ページを作成しても、参照されるのはページ1のみ。

drawio側を更新してもmarkdown側には即反映ではない？  
⇒ プレビューに反映されないだけみたい。html出力には反映された。  
⇒⇒ MPEを利用しているなら右上から更新すればいい  

### PlantUML

```plantuml
@startuml
hide empty description
[*] --> State1
State1 --> [*]
State1 : this is a string
State1 : this is another string

State1 -> State2
State2 --> [*]
@enduml
```
