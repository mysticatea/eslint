# ESLint

[![Gitter](https://badges.gitter.im/mysticatea/eslint.svg)](https://gitter.im/mysticatea/eslint?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

このリポジトリは [ESLint](https://github.com/eslint/eslint) に関するバグ報告・機能提案・質問を日本語で行える場所です。

ESLint に関することなら、何でもお気軽に [Issue](https://github.com/mysticatea/eslint/issues/new) を作ってみてください。

例えば、

- バグっぽい動作を見つけた
- こんな機能 / ルールがほしい
- この機能を日本語で解説して欲しい
- ○○したいんだけど、どうすればいいの?

オープンソース プロジェクトにとってユーザーの声は財産です。
どうぞよろしくお願いします。

----

以下は README.md の一部です。

## インストール方法

ESLint は npm を使ってインストールします。

    npm install -g eslint

## 使い方

最初に `--init` オプションを利用して設定ファイルを作ります。

    eslint --init

そして、任意の JS コードに対して eslint コマンドを実行します。

    eslint test.js test2.js

## 設定ファイル

`eslint --init` コマンドを実行すると、`.eslintrc` ファイルが作成されます。
`.eslintrc` ファイルによって、どんなルールで JS コードを検証するかを設定することができます。

```json
{
    "extends": "eslint:recommended",
    "rules": {
        "semi": [2, "always"],
        "quotes": [2, "double"]
    }
}
```

`"semi"` と `"quotes"` はルール名です ([ルール一覧](http://eslint.org/docs/rules) (英語))。
`2` とあるのは各ルールの警告レベルを設定しています。

* `0` - ルールをオフにします。
* `1` - 警告にします (ルール違反を見つけても `eslint` コマンドは正常終了します)。
* `2` - エラーにします (ルール違反を見つけたら `eslint` コマンドは exit code 1 で終了します)。

これらのルール・レベルによって、ESLint のふるまいを細やかに制御できます。
設定項目についての詳細は [configuration docs](http://eslint.org/docs/user-guide/configuring) (英語) を参照ください。

## スポンサー

* Development is sponsored by [Box](https://box.com)
* Site search ([eslint.org](http://eslint.org)) is sponsored by [Algolia](https://www.algolia.com)

## 開発チームについて

* Nicholas C. Zakas ([@nzakas](https://github.com/nzakas)) - project lead
* Ilya Volodin ([@ilyavolodin](https://github.com/ilyavolodin)) - reviewer
* Brandon Mills ([@btmills](https://github.com/btmills)) - reviewer
* Gyandeep Singh ([@gyandeeps](https://github.com/gyandeeps)) - reviewer
* Mathias Schreck ([@lo1tuma](https://github.com/lo1tuma)) - committer
* Jamund Ferguson ([@xjamundx](https://github.com/xjamundx)) - committer
* Ian VanSchooten ([@ianvs](https://github.com/ianvs)) - committer
* Toru Nagashima (長島 徹) ([@mysticatea](https://github.com/mysticatea)) - committer
* Burak Yiğit Kaya ([@byk](https://github.com/byk)) - committer
* Alberto Rodríguez ([@alberto](https://github.com/alberto)) - committer

## リリース スケジュールについて

ESLint は隔週リリースされています。
