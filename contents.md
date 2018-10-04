# Clean Architecture
# 定期輪読会

### Chapter.30 - 34

</br>

2018-11-08

@orepuri

---

## Chapter30. データベースは詳細

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter30. データベースは詳細
</div>
</br>


データベースはアーキテクチャの構成要素ではない

独立した1つのソフトウェアであり, データアクセスを提供する道具

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter30. データベースは詳細
</div>
</br>


下位レベルの仕組み

アーキテクチャが下位に汚染されることは許されない

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter30. データベースは詳細
</div>
</br>


### データベースフレームワーク(ORM)
</br>

行やテーブルをオブジェクトとして受け渡す

アーキテクチャ的には間違っている

ユースケースやビジネスルール, UIが</br>
リレーショナルデータ構造に縛られる



---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter30. データベースは詳細
</div>
</br>


### もしディスクがなかったら?
</br>


すべてのデータがRAMに格納されるようになっても</br>
表形式にしてSQLでアクセスするか?

リンクリストやツリー, ハッシュなどのデータ構造や</br>
オブジェクトへの参照を使ってアクセスする

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter30. データベースは詳細
</div>
</br>


### パフォーマンスは?
</br>


アーキテクチャ的にも気になるが, データアクセスのパフォーマンスは</br>
ビジネスルールと切り離して考える

データアクセスのパフォーマンスは下位レベルの関心事

システム全体のアーキテクチャとは関係ない

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter30. データベースは詳細
</div>
</br>


### 30章 まとめ
</br>


データ構造であるデータモデルはアーキテクチャ的に重要

データが保存されるデバイスや表現形式はアーキテクチャ的に重要ではない

データ（モデル）が重要であり, データベースは詳細に過ぎない


---

## Chapter31. ウェブは詳細

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter31. ウェブは詳細
</div>

## 止まらない振り子
</br>

メインフレーム

インターネットとブラウザ

動的コンテンツ

Web2.0

Node.js

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter31. ウェブは詳細
</div>

## アーキテクトの視点
</br>

長期的な観点

短期的な振り子に振り回されたくない

ビジネスルールの中心から切り離す


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter31. ウェブは詳細
</div>

## 31章 まとめ
</br>

GUIは詳細であり, WebはGUI

GUIは詳細

Webを入出力デバイスの一種と捉える


---
## Chapter32. フレームワークは詳細

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

フレームワークはアーキテクチャではない

</br>

フレームワーク作者はユーザーのアプリケーションとの結合を望む

長期的な約束がない一方でリスクと負担を背負わなければならない</br>
(利便性の代償)

一方的な結婚

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

## リスク
</br>

フレームワークのアーキテクチャに難がある

フレームワークの機能が不足してくる

フレームワークが希望しない方向に進化する

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

## 解決策
</br>

フレームワークと強く結合しないこと

アーキテクチャをエンティティやユースケースの</br>
外側にあるものとみなす


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

## 解決策
</br>

フレームワークと強く結合しないこと

アーキテクチャをエンティティやユースケースの</br>
外側にあるものとみなす

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

## 今あなたたちを夫婦として宣言する
</br>

どうしても結婚するしかない状況がある

使うと決めた時点で縛られることを認識すること

どんなときでも使うことになる

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

# 結婚は慎重に


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter32. フレームワークは詳細
</div>

## 32章 まとめ
</br>

フレームワークとすぐに結婚しようとしてはいけない

できる限り時間を稼ぐこと

アーキテクチャの境界から遠ざける

---
## Chapter33. 事例: 動画販売サイト

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter33. 事例: 動画販売サイト
</div>

優れたアーキテクトが使う手順や判断

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter33. 事例: 動画販売サイト
</div>

*ユースケース分析*

アクターとユースケースと洗い出し

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter33. 事例: 動画販売サイト
</div>


*コンポーネントアーキテクチャ*

コンポーネントの設計

細かく分割して設計/実装する

ビルドやデプロイは選択肢として残す

依存性の管理もしっかり

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter33. 事例: 動画販売サイト
</div>


## 33章 まとめ

図 33-2 のアーキテクチャ図

2つの分割軸

単一責任の原則に基づくアクターによる分割

依存性のルールによる分割

変更やデプロイに対する柔軟性

---
## Chapter34. 書き残したこと

by Simon Brown

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## レイヤーによるパッケージング
</br>

Web, ビジネスロジック, 永続化の3つのレイヤーに分ける

水平方向の分離

規模が大きくなるとより細かいモジュール化が必要

ビジネスドメインについて何も叫ばない


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## 機能によるパッケージング
</br>

ユースケースごとにレイヤーを分ける

垂直方向の分離

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## ポートとアダプター
</br>

ドメインを表現する内側と, 外部とのインタラクションを行う外側に分離

DDD

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## コンポーネントによるパッケージング
</br>

ゆるいレイヤードアーキテクチャの例

コントローラから直接レポジトリを使用

ビジネスロジックと永続化をまとめてコンポーネントにする

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## 悪魔は実装の詳細に宿る
</br>

Javaのような言語でpublic修飾子を使いすぎる

アーキテクチャのスタイルに違反したコードが防げなくなる

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## 組織化かカプセル化か
</br>

すべてをpublicにするとパッケージは単なるグルーピング

カプセル化ができなくなりパッケージの意味がない


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## そのほかの分割方法
</br>

Java9以降のモジュールシステム

別のソースコードツリー（Gitレポジトリ）

SBTサブプロジェクト


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter34. 書き残したこと
</div>

## 34章 まとめ
</br>

いい設計をしても実装がまずければダメになる

悪魔は実装の詳細に宿る

