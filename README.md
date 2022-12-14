# TemplateRepository
Gitリポジトリを作成する上で、テンプレートになるようなファイル/設定を置いとくところ。

# ツール情報
・Unity 20XX.X.XX

・Source Tree

# ブランチに関するルール
## master ブランチ
リポジトリ生成時に最初に生成されるブランチ。

α版やβ版など大きなバージョン毎の差分のみを持ちます。

バージョン毎にdevelopブランチをマージし、更新します。


<b>絶対にこのブランチにプッシュしないでください。developへのマージ専用です。</b>

## develop ブランチ
最新の開発状況を維持するブランチ。

featureブランチでの作業が終了し、<b>不具合も無い状態</b>になったら

該当featureブランチをマージさせる事で、常に最新の状態にする。

## feature ブランチ
各作業ごとに分かれたブランチ。

前述するブランチと異なり、複数存在する。

作業が割り充てられた際に、developブランチを切り作成する。

作業が終了し、developブランチからのマージが完了した際は<b>このブランチを削除する事。</b>

>・featureブランチの命名規則
>
>feature/["作業者氏名"]/["作業内容"]
>
>例) feature/Yamada/CharacterMove

# 更新作業の大体の流れ
1. 仕事を貰う。
2. developブランチを更新する。(フェッチ)
3. featureブランチをdevelopブランチを切り作成する。
4. 作業する。(コミット&プッシュ)
5. developブランチに作業したfeatureブランチをマージする。
※ feature → developではなく、develop → featureです。
6. そのブランチでの作業が無い場合、作業していたfeatureブランチを削除する。
7. 1に戻る

# 参考リンク
命名規則: https://takap-tech.com/entry/2020/03/08/015721
 
