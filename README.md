# mtml-autocomplete-IntelliJ-IDEA

IntelliJ IDEA で Movable Type のテンプレートタグの入力を保管してくれる Live template です。

## インストール

MTML.xml 下記のディレクトリに保存してください。 `IntelliJIdea2018.3` 部分はご利用のバージョンによって異なります。

```
/Users/ユーザー名/Library/Preferences/IntelliJIdea2018.3/templates/MTML.xml
```

もし、 `VSC > Sync Settings` で環境設定をリポジトリに同期している場合は、保存先のパスは下記となります。

```
/Users/ユーザー名/Library/Preferences/IntelliJIdea2018.3/settingsRepository/repository/templates/MTML.xml
```

もし、 `File > IDE Settings Sync` で JetBrains アカウントを利用して環境設定を同期している場合は、保存先のパスは下記となります。

```
/Users/ユーザー名/Library/Preferences/IntelliJIdea2018.3/jba_config/templates/MTML.xml
```

あらかじめ IntelliJ IDEA を終了しておき、インストール後に起動するとスムーズに反映されるようです。

## 使い方

テンプレートタグは `<mtentri` のように入力すると候補が現れます。

グローバルモディファイアも普通に入力すると候補が現れますが、条件によっては現れないので、その場合は `Command + J` で手動で呼び出します。

環境変数は `mtconfig` と入力すると候補が現れますが、条件によっては現れないので、その場合は `Command + J` で手動で呼び出します。なお、候補には `mtdonfig-AdminCGIPath` と表示されますが、ハイフンは入力しなくても問題ありませんし、エンターを押して入力される値には `mt-donfig-` は付きません。

テンプレートを見やすくするための見出し的なコメントは、 `mtmlhead1` `mtmlhead2` `mtmlhead3` で呼出せます。