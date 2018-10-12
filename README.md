# Matrices in SATySFi!

[日本語版はこちら][README-ja.md]

## Usage

```satysfi
+math(${
  \matrix![
    [$(1); $(2); $(3)];
    [$(4); $(5); $(6)];
    [$(7); $(8); $(9)];
  ]
});
```

This code will produce the following.

[![A 3x3 matrix that is {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}}][sample_matrix.png]][sample_matrix.png]

More precisely, this library provides a math command `\matrix : [(math list) list] math-cmd`. You can pass 2d (rectangular) list into this command.

See [`example`][example] for more complicated examples.

## Notice

**CAUTION**: This library is tested only under SATySFi 0.0.3. Since SATySFi is under the initial development period, any compatibility is ensured for future versions of SATySFi.

## Installation

Just copy `matrix.satyh` under your `LIBROOT/dist/packages/` (LIBROOT changes depending on your environment).

### Example: Unix-like OSs

```sh
git clone https://github.com/nekketsuuu/satysfi-matrix.git
cd satysfi-matrix
cp matrix.satyh ~/.satysfi/dist/packages/
```

### Example: Windows

```sh
git clone https://github.com/nekketsuuu/satysfi-matrix.git
cd satysfi-matrix
copy matrix.satyh %USERPROFILE%\.satysfi\dist\packages\
```

## Uninstallation

Delete `LIBROOT/dist/packages/matrix.satyh`.

## Known Issues

See [GitHub Issues].

## Contributing

Both pull requests and issues are welcome! Please write them in English or in Japanese.

Also, this library is distributed under The Unlicense. You can freely edit and use this library.


  [README-ja.md]: https://github.com/nekketsuuu/satysfi-matrix/blob/master/README-ja.md
  [sample_matrix.png]: https://raw.githubusercontent.com/nekketsuuu/satysfi-matrix/master/doc/img/sample_matrix.png
  [example]: https://github.com/nekketsuuu/satysfi-matrix/blob/master/example
  [GitHub Issue]: https://github.com/nekketsuuu/satysfi-matrix/issues
