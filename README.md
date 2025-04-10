# catpow-scss

catpow-scssは色やサイズの設定設定値を複数のscssファイルで共有するためのmixin集です。
2〜3文字の短い名前のmixinで、複数のプロパティを同じく2〜3文字の短い名前で指定して設定します。


## Install

```shell
git submodule add https://github.com/synchrovision/catpow-scss.git scss/catpow
```


## INDEX

### Main Mixin
| |プロパティ|概要|Document|GitHub|
|:--|:--|:--|:-:|:-:|
|**anm**|animation|アニメーション関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/anm/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_anm.scss#L1-L24)|
|**bdr**|border border-radius|ボーダー関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/bdr/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_bdr.scss#L1-L24)|
|**bg**|background background-image background-position background-size|背景色、背景画像、グラデーション|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/bg/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_bg.scss#L1-L87)|
|**bnd**|display position width height margin padding overflow object-fit object-position|レイアウト・サイズ・余白を設定|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/bnd/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_bnd.scss#L1-L197)|
|**bp**|@media|画面幅によるメディアクエリ|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/bp/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_bp.scss#L1-L19)|
|**clp**|clip-path|クリッピングパスを生成|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/clp/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_clp.scss#L1-L141)|
|**cnt**|counter-reset counter-increment content|カウンターの表示|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/cnt/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_cnt.scss#L1-L52)|
|**col**|column column-rule column-gap|カラムサイズとカラム境界線の設定|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/col/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_col.scss#L1-L10)|
|**ctn**|@container|コンテナクエリ|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/ctn/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_ctn.scss#L1-L64)|
|**flx**|flex justify-content align-content justify-items align-items|フレックスレイアウト関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/flx/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_flx.scss#L1-L51)|
|**grd**|grid|グリッドレイアウト関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/grd/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_grd.scss#L1-L91)|
|**msk**|mask-image mask-border|画像による切り抜き|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/msk/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_msk.scss#L1-L20)|
|**shd**|box-shadow text-shadow|ドロップシャドウ関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/shd/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_shd.scss#L1-L130)|
|**svg**|fill stroke text-anchor dominant-baseline|SVG関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/svg/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_svg.scss#L1-L42)|
|**tbl**|table-layout border-collapse border-spacing|テーブル関連|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/tbl/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_tbl.scss#L1-L18)|
|**trn**|transition transform mix-blend-mode filter animation perspective|トランジション、変形、透明|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/trn/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_trn.scss#L1-L95)|
|**txt**|text-align font-size line-height font-family color vertical-align|文字揃え、文字サイズ、文字色|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/txt/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_txt.scss#L1-L66)|
|**plh**|::placeholder|プレースホルダーの文字サイズ、文字色など|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/plh/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_txt.scss#L67-L80)|
|**usr**|cursor pointer-event user-select|カーソル、ユーザー操作・選択の受付|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/main/usr/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_usr.scss#L1-L26)|

### mixin
| |概要|Document|GitHub|
|:--|:--|:-:|:-:|
|**default_break**|ブラウザのデフォルトの余白や境界線の設定、モバイルブラウザの文字サイズ調整などをなくし、ブラウザによる表示の差異を抑制します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/default_break/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L1-L5)|
|**hide_scrollbar**|スクロールバーを非表示にします。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/hide_scrollbar/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L6-L12)|
|**define_color_vars**|get_color_vars関数が定義されている場合に、引数の色の値のマップまたはグローバル変数$colorsを元にそれらのCSS変数を:rootに定義するコードを出力します。catpow-ssg環境下では各色をhslaに分解したCSS変数が定義されます。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/define_color_vars/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L13-L25)|
|**define_color_classes**|get_color_classes関数が定義されている場合に、引数の色の値のマップまたはグローバル変数$colorsを元に色の設定を行うクラスを定義するコードを出力します。catpow-ssg環境下ではdefine_color_varsによって各CSS変数が定義されていることを前提に、12段階で色相を分割した各色のクラスを定義します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/define_color_classes/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L32-L47)|
|**clear_float**|回り込み解除のスタイルを適用します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/clear_float/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L48-L50)|
|**clear_fix**|フロートレイアウトのコンテナのafter擬似要素に回り込み解除のスタイルを適用します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/clear_fix/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L51-L53)|
|**pull_left**|左回り込みのスタイルを適用します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/pull_left/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L54-L56)|
|**pull_right**|右回り込みのスタイルを適用します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/pull_right/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L57-L60)|
|**flex_equalize**|子要素の数によってflex-basisを調整し、行ごとの要素数の差が１以上にならないようにします。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/flex_equalize/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_flx.scss#L52-L106)|
|**gradient**|グラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/gradient/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L1-L9)|
|**linear-gradient**|線型グラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/linear-gradient/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L10-L20)|
|**radial-gradient**|円形グラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/radial-gradient/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L21-L28)|
|**shade**|陰によって立体感を表現するグラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/shade/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L29-L32)|
|**glass**|ガラスのような光沢を表現するグラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/glass/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L33-L42)|
|**mist**|うっすらとかかるもやを表現するグラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/mist/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L43-L46)|
|**stripe**|縞模様を表現するグラデーションを作成します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/stripe/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_gradient.scss#L47-L51)|
|**round_table**|表の４隅を角丸にします。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/round_table/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_tbl.scss#L19-L34)|
|**text-decoration**|下線や打ち消し線などのテキスト装飾を短縮表現の値のリストで設定します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/text-decoration/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_txt.scss#L81-L119)|
|**text-emphasis**|テキストの圏点を短縮表現の値のリストで設定します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/text-emphasis/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_txt.scss#L120-L154)|
|**wp_admin_color**|wordpressのwp-admin/css/colors/_variables.scssで定義されるSCSS変数を一括で定義します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/mixin/wp_admin_color/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_wp.scss#L1-L45)|

### function
| |概要|Document|GitHub|
|:--|:--|:-:|:-:|
|**is_quoted**|変数がクオート付の文字列であるかを判定します。正確にはget_real_typeの関数が存在する場合に、get_real_typeから得られる値の型がstringであるかを判定します。scssphpではクオートで括られていない文字列の型はstringではなくkeywordです。get_real_typeが定義されていない環境下では単にstring型であるかどうかの判定をします。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/is_quoted/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L26-L31)|
|**tint**|色の濃さを変更してrgb形式で返します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/tint/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L61-L88)|
|**ease**|animation-timing-functionやtransition-timing-functionで用いるイージングのキーワードやeasing-funcitonを返します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/ease/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L89-L108)|
|**replace_values**|第一引数の値、もしくはリスト内の値を、第二引数のマップに基づいて置き換えます。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/replace_values/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L109-L123)|
|**fill_4_values**|値が４つ未満のリストをmarginやpaddingの値の補完と同様のルールで４つの値をもつリストに補完します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/fill_4_values/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L124-L146)|
|**img**|background-imageなどで用いる画像URLの値を返します。グローバル変数$imagesが定義されていればそこから画像のURLの値を取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/img/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L147-L169)|
|**sel**|グローバル変数$selectorsを用いてセレクタの値を置き換えます。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/sel/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L170-L183)|
|**clr**|colorやbackground-colorなどで用いる色の値を返します。translate_color関数が定義されていればその関数から、グローバル変数$colorsが定義されていればそれから色の値を取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/clr/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L184-L204)|
|**sz**|widthやheightなどで用いるサイズの値を返します。translate_size関数が定義されていればその関数から、グローバル変数$sizesが定義されていればそれからサイズの値を取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/sz/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L205-L226)|
|**szs**|marginやpaddingなどで用いるサイズの値のリストを返します。translate_size関数が定義されていればその関数から、グローバル変数$sizesが定義されていればそれからサイズの値のリストを取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/szs/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L227-L240)|
|**wt**|font-weightで用いる文字の太さを表す値を名を返します。 translate_weight関数が定義されていればその関数から、グローバル変数$weightsが定義されていればそれから文字の太さの値を取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/wt/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L241-L252)|
|**fnt**|font-familyで用いるフォント名を返します。translate_font関数が定義されていればその関数から、グローバル変数$fontsが定義されていればそれからフォント名を取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/fnt/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L253-L262)|
|**slice**|リストから範囲を指定して部分を取り出し新たなリストを取得します。|[![Document](https://img.shields.io/badge/Document-666)](https://catpow.info/products/scss/reference/function/slice/)|[![Code](https://img.shields.io/badge/Code-CC6699?logo=sass&logoColor=fff)](https://github.com/synchrovision/catpow-scss/blob/master/src/_basic.scss#L263-L275)|


