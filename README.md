# table highlighting with CSS :has()

`table` のセルを `:hover` したり、セル内の要素に `:focus` したときに、そのセルをわかりやすくハイライト表示する CSS のサンプルを紹介しています。

```
src/styles/styles.css
```

スタイルは上記のファイルにまとまっています。

Tailwind CSS を使用しているため `@apply` 以降の指定は実際のプロパティと値に読みかえてください。

通常の CSS にしたものを下記に入れてあります。参考まで。

```
css-sample/styles.css
```

なお、サンプルの CSS は、同じくサンプルで使用している `table` の構造（例えば `thead` や `tbody` 要素のあるなし、行や列の数など）が前提で書かれています。

`table` 構造を大きく変えると、CSS もそれに合わせて書き換えないといけませんので注意してください。

また、フォーカス時の動作に関しては、下記のデモだとセル内にフォーカス可能な要素を置いていないため確認できません。

お手元で、例えば `button` や `a` 要素など、フォーカスを受け取る要素を `td` 内に入れて確認してみてください。

CSS 上では `:focus-within` に対するスタイルも指定してあるので、セル内の要素がフォーカスを受け取れば、`:hover` 同様にハイライト処理がされます。

## デモ

- [:hover や :focus でセルをわかりやすくハイライトする CSS のサンプル - table highlighting with CSS :has()](https://burnworks.github.io/table-hover-highlighting-css/)

## 謝辞

以下の X ポストからヒントをいただきました。

- [https://x.com/jh3yy/status/1887245206418038860](https://x.com/jh3yy/status/1887245206418038860)
