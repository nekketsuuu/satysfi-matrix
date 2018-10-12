# SATySFi で行列！

[English version is here.][README.md]

## 使い方

```satysfi
+math(${
  \matrix![
    [${1}; ${2}; ${3}];
    [${4}; ${5}; ${6}];
    [${7}; ${8}; ${9}];
  ]
});
```

このコードが下のようになります。

[![3x3 型行列です。要素は {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}} です。][sample_matrix.png]][sample_matrix.png]

より正確には、このライブラリは math モードで使えるコマンド `\matrix : [(math list) list] math-cmd` を提供します。(長方形型の) 2次元リストを渡すことでコマンドを使用できます。

より複雑な例は [`example`][example] をご覧ください。

## 注意

**注意**: このライブラリは SATySFi 0.0.3 でのみテストされています。現在 SATySFi は開発初期であるため、SATySFi のバージョンアップに対するこのライブラリの互換性は一切保証しません。

## インストール方法

`matrix.satyh` を `LIBROOT/dist/packages/` 下へコピーしてください (LIBROOT は環境によって変わります)。

### 例: Unix 系 OS

```sh
git clone https://github.com/nekketsuuu/satysfi-matrix.git
cd satysfi-matrix
cp matrix.satyh ~/.satysfi/dist/packages/
```

### 例: Windows

```sh
git clone https://github.com/nekketsuuu/satysfi-matrix.git
cd satysfi-matrix
copy matrix.satyh %USERPROFILE%\.satysfi\dist\packages\
```

## アンインストール方法

LIBROOT/dist/packages/matrix.satyh` を削除してください。

## 既知の問題

[GitHub Issues] をご覧ください。

## 貢献

Pull request も issue 報告も歓迎しています！　英語でも日本語でも大丈夫です。

また、このライブラリは The Unlicense の元で配布しています。自由に編集・使用することができます。


  [README.md]: https://github.com/nekketsuuu/satysfi-matrix/blob/master/README.md
  [sample_matrix.png]: https://raw.githubusercontent.com/nekketsuuu/satysfi-matrix/master/doc/img/sample_matrix.png
  [example]: https://github.com/nekketsuuu/satysfi-matrix/blob/master/example
  [GitHub Issues]: https://github.com/nekketsuuu/satysfi-matrix/issues
