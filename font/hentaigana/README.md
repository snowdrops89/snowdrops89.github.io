# ninjal_hentaigana.woffについて
　NINJAL変体仮名フォントは、国立国語研究所で配布されている変体仮名のフォントです。

　変体仮名（U+1B001～U+1B11E）のみのフォントです。

> [NINJAL変体仮名フォント - 学術情報交換用変体仮名 | 国立国語研究所](https://cid.ninjal.ac.jp/kana/font/)

## 1B000.woff について
　上記フォント未収録だった（U+1B000）を『花園明朝A』よりサブセットフォント化したもの。

　一文字だけです～。NINJAL変体仮名フォントとセットで使います。

```
@font-face {
    font-family:NINJAL変体仮名;
    src: url('font/hentaigana/ninjal_hentaigana.woff') format('woff');
}
@font-face {
    font-family:変体仮名1B000;
    src: url('font/hentaigana/1B000.woff') format('woff') ;
}

.NINJAL {
    font-family: NINJAL変体仮名,変体仮名1B000;
}
```

# HanaMin_hentaigana.woffについて

　『花園明朝A』より変体仮名部分（U+1B000～U+1B11E）のみをサブセットフォント化したもの。

　本体は以下にあります。

> [花園フォント](http://fonts.jp/hanazono/)

```
@font-face {
    font-family:花園明朝変体仮名;
    src: url('hentaigana/HanaMin_hentaigana.woff') format('woff');
}
.hanazono {
    font-family: 花園明朝変体仮名;
}
```
