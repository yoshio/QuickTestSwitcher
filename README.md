Quick Test Switcher
===================

テストコードと実装コードを簡単に切り替えられるようにするためのVisual Studio用アドインです。

Quick JUnit Plugin for Eclipseにインスパイアされて作りました。
まだコードを切り替えるくらいしかできません。

インストール方法
----------------

リリースされたものをインストールするもっとも簡単な方法は、
Visual Studioの拡張機能マネージャで、「QuickTestSwitcher」を検索してインストールする方法です。

ソースコードからインストールしたい場合、

1. コードを取得する
1. QuickTestSwitcher.slnを開く
1. Releaseでビルドする
1. QuickTestSwitcher\bin\Release\QuickTestSwitcher.vsixをダブルクリックして実行する

とする必要があります。
また、すでにQuickTestSwitcherがインストール済みの場合は、
アンインストールするか、vsmanifestのVersionを増やしてビルドする必要があります。

使い方
------

コードを開いた状態で、Ctrlキーと0(ゼロ)を同時に押すだけです。
対応するファイル(テスティングペア)があれば、それを開きます。

本当は本家と合わせて、Ctrl-9に割り当てたかったのですが、
上手くマッピングできなかったので仕方なくCtrl-0に割り当てました。
本家でCtrl-0はテストの実行に割り当てられていますが、
テストは別アドインでビルド時にバックグラウンドで走らせたい、
という思惑があるのでこの機能は実装しません。
EclipseとVSを行ったり来たりする人にとっては混乱の元かもしれませんが、
いいマッピングを思いつかなかったのでとりあえずこれで行きます。

詳しくは
--------

[マニュアル](http://bleis-tift.github.com/QuickTestSwitcher/)をご覧ください。
