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
  - [pythonインストール](#pythonインストール)
    - [Pythonのバージョンについて](#pythonのバージョンについて)
    - [インストーラの入手](#インストーラの入手)
  - [章立て](#章立て)

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

## pythonインストール

以下順序でPythonのインストールを進める。  

1. 利用するバージョンについて
1. インストーラの入手
1. インストーラの実行
1. インストールできたことの確認

### Pythonのバージョンについて

Pythonには大まかに2.n系と3.n系が存在する。  
それぞれの主な特徴は下図の通り。  

![Ver](./img/01Python/01.drawio.png)

どちらを利用することもありうるが、本書では最新のPython環境を利用する。  

:::info
Pythonには派生形が多数存在する。  
・Circuit Python  
・Micro Python  
・Iron Python  
これらと区別するためにPython.orgからダウンロードできるPythonをCPythonと呼称することもある。
:::

:::note
筆者が現在利用しているメイン機では2.7, 3.7～3.11をインストールしている。  
このため、利用するバージョンを使い分ける手段が必要になる。  
バージョンを使い分ける手段は後述する。  
:::

### インストーラの入手

以下Python.orgのページからインストーラをダウンロードする。  
[https://www.python.org/](https://www.python.org/)

Downloadsをクリックする。

![画像jpg](./img/01Python/10.png){.image_w900}

トップには最新バージョンが表示されるハズなのでクリックする。

![画像jpg](./img/01Python/11.png){.image_w900}

ブラウザのダウンローダに従って、名前を付けて保存する。

![画像jpg](./img/01Python/12.png){.image_w900}

適当なフォルダへ保存する。  
下図は一例として「ダウンロード」フォルダへ、そのままのファイル名で保存している。  

![画像jpg](./img/01Python/13.png){.image_w900}

## 章立て

pythonインストール

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
