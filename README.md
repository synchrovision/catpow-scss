# cawpow-scss

catpow-scssはscssのコードを短く手早く書くことを目的としたmixin集です。
catpow-scssはmixinは2〜3文字の短い名前で、複数のプロパティを同じく2〜3文字の短い名前で指定して設定できます。

```command
git submodules add https://github.com/synchrovision/cawpow-scss scss/catpow
```

## sample

```scss
@import "config/style_config.scss";

.wp-block-embed-youtube{
	@include bnd((d:b,w:f 100rem,mg:0 a));
	.wp-block-embed__wrapper{
		@include bnd((d:b,p:r));
		iframe{
			@include bnd((d:b,p:a,t:0,b:0,l:0,r:0,h:f,w:f));
		}
	}
	&.wp-embed-aspect-16-9{
		.wp-block-embed__wrapper{
			@include bnd((pdt:56.25%));
		}
	}
}
```
↓
```css
@charset "utf-8";
.wp-block-embed-youtube {
	display: block;
	max-width: 100rem;
	width: 100%;
	margin: 0px auto;
}
.wp-block-embed-youtube .wp-block-embed__wrapper {
	display: block;
	position: relative;
}
.wp-block-embed-youtube .wp-block-embed__wrapper iframe {
	display: block;
	position: absolute;
	top: 0px;
	bottom: 0px;
	left: 0px;
	right: 0px;
	height: 100%;
	width: 100%;
}
.wp-block-embed-youtube.wp-embed-aspect-16-9 .wp-block-embed__wrapper {
	padding-top: 56.25%;
}
```


# Mixin一覧

## anm

<table>
    <tbody>
        <tr>
            <th rowspan='7'>a</th>
            <td rowspan='7'>animation</td>
            <th>i</th>
            <td>infinite</td>
        </tr>
        <tr>
            <th>r</th>
            <td>reverse</td>
        </tr>
        <tr>
            <th>a</th>
            <td>alternate</td>
        </tr>
        <tr>
            <th>e</th>
            <td>ease</td>
        </tr>
        <tr>
            <th>l</th>
            <td>linear</td>
        </tr>
        <tr>
            <th>f</th>
            <td>forwards</td>
        </tr>
        <tr>
            <th>b</th>
            <td>backwards</td>
        </tr>
        <tr>
            <th>dur</th>
            <td>animation-duration</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>del</th>
            <td>animation-delay</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>dir</th>
            <td>animation-direction</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='14'>e</th>
            <td rowspan='14'>animation-timing-function</td>
            <th>l</th>
            <td>linear</td>
        </tr>
        <tr>
            <th>e</th>
            <td>ease</td>
        </tr>
        <tr>
            <th>i</th>
            <td>ease-in</td>
        </tr>
        <tr>
            <th>o</th>
            <td>ease-out</td>
        </tr>
        <tr>
            <th>io</th>
            <td>ease-in-out</td>
        </tr>
        <tr>
            <th>ib</th>
            <td>cubic-bezier(0.6 0.3 0.8 -1.0)</td>
        </tr>
        <tr>
            <th>b</th>
            <td>cubic-bezier(0.2 2.0 0.4 0.7)</td>
        </tr>
        <tr>
            <th>ob</th>
            <td>cubic-bezier(0.2 2.0 0.4 0.7)</td>
        </tr>
        <tr>
            <th>iob</th>
            <td>cubic-bezier(0.3 -0.5 0.7 1.5)</td>
        </tr>
        <tr>
            <th>ij</th>
            <td>cubic-bezier(0.2 -10.0 0.8 -10.0)</td>
        </tr>
        <tr>
            <th>j</th>
            <td>cubic-bezier(0.2 10.0 0.8 10.0)</td>
        </tr>
        <tr>
            <th>oj</th>
            <td>cubic-bezier(0.2 10.0 0.8 10.0)</td>
        </tr>
        <tr>
            <th>ioj</th>
            <td>cubic-bezier(0.2 -10.0 0.8 10.0)</td>
        </tr>
        <tr>
            <th>u</th>
            <td>cubic-bezier(0 .8 1 .2)</td>
        </tr>
        <tr>
            <th rowspan='1'>i</th>
            <td rowspan='1'>animation-iteration-count</td>
            <th>i</th>
            <td>infinite</td>
        </tr>
        <tr>
            <th rowspan='2'>f</th>
            <td rowspan='2'>animation-fill-mode</td>
            <th>f</th>
            <td>forwards</td>
        </tr>
        <tr>
            <th>b</th>
            <td>backwards</td>
        </tr>
        <tr>
            <th>p</th>
            <td>animation-play-state</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## bdr

<table>
    <tbody>
        <tr>
            <th rowspan='4'>p</th>
            <td rowspan='4'>[線の位置]</td>
            <th>l</th>
            <td>left</td>
        </tr>
        <tr>
            <th>r</th>
            <td>right</td>
        </tr>
        <tr>
            <th>t</th>
            <td>top</td>
        </tr>
        <tr>
            <th>b</th>
            <td>bottom</td>
        </tr>
        <tr>
            <th>c</th>
            <td>color</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>w</th>
            <td>width</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>s</th>
            <td>style</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='3'>i</th>
            <td rowspan='3'>border-image</td>
            <th>s</th>
            <td>stretch</td>
        </tr>
        <tr>
            <th>r</th>
            <td>round</td>
        </tr>
        <tr>
            <th>f</th>
            <td>fill</td>
        </tr>
        <tr>
            <th>r</th>
            <td>border-radius</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## bg

<table>
    <tbody>
        <tr>
            <th>i</th>
            <td>background-image</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>c</th>
            <td>background-color</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='5'>r</th>
            <td rowspan='5'>background-repeat</td>
            <th>n</th>
            <td>no-repeat</td>
        </tr>
        <tr>
            <th>x</th>
            <td>repeat-x</td>
        </tr>
        <tr>
            <th>y</th>
            <td>repeat-y</td>
        </tr>
        <tr>
            <th>xy</th>
            <td>repeat</td>
        </tr>
        <tr>
            <th>r</th>
            <td>repeat</td>
        </tr>
        <tr>
            <th rowspan='2'>a</th>
            <td rowspan='2'>background-attachment</td>
            <th>f</th>
            <td>fixed</td>
        </tr>
        <tr>
            <th>s</th>
            <td>scroll</td>
        </tr>
        <tr>
            <th rowspan='6'>s</th>
            <td rowspan='6'>background-size</td>
            <th>fit</th>
            <td>100% 100%</td>
        </tr>
        <tr>
            <th>cnt</th>
            <td>contain</td>
        </tr>
        <tr>
            <th>cvr</th>
            <td>cover</td>
        </tr>
        <tr>
            <th>f</th>
            <td>100% 100%</td>
        </tr>
        <tr>
            <th>c</th>
            <td>cover</td>
        </tr>
        <tr>
            <th>i</th>
            <td>contain</td>
        </tr>
        <tr>
            <th rowspan='5'>p</th>
            <td rowspan='5'>background-position</td>
            <th>l</th>
            <td>left</td>
        </tr>
        <tr>
            <th>r</th>
            <td>right</td>
        </tr>
        <tr>
            <th>t</th>
            <td>top</td>
        </tr>
        <tr>
            <th>b</th>
            <td>bottom</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th rowspan='4'>cl</th>
            <td rowspan='4'>background-clip</td>
            <th>b</th>
            <td>border-box</td>
        </tr>
        <tr>
            <th>p</th>
            <td>padding-box</td>
        </tr>
        <tr>
            <th>c</th>
            <td>content-box</td>
        </tr>
        <tr>
            <th>t</th>
            <td>text</td>
        </tr>
    </tbody>
</table>


## bnd

<table>
    <tbody>
        <tr>
            <th rowspan='13'>d</th>
            <td rowspan='13'>display</td>
            <th>b</th>
            <td>block</td>
        </tr>
        <tr>
            <th>f</th>
            <td>flex</td>
        </tr>
        <tr>
            <th>g</th>
            <td>grid</td>
        </tr>
        <tr>
            <th>ib</th>
            <td>inline-block</td>
        </tr>
        <tr>
            <th>i</th>
            <td>inline</td>
        </tr>
        <tr>
            <th>it</th>
            <td>inline-table</td>
        </tr>
        <tr>
            <th>t</th>
            <td>table</td>
        </tr>
        <tr>
            <th>th</th>
            <td>table-header-group</td>
        </tr>
        <tr>
            <th>tb</th>
            <td>table-row-group</td>
        </tr>
        <tr>
            <th>tf</th>
            <td>table-footer-group</td>
        </tr>
        <tr>
            <th>tr</th>
            <td>table-row</td>
        </tr>
        <tr>
            <th>tc</th>
            <td>table-cell</td>
        </tr>
        <tr>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th rowspan='2'>ap</th>
            <td rowspan='2'>appearance</td>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th>b</th>
            <td>button</td>
        </tr>
        <tr>
            <th rowspan='4'>p</th>
            <td rowspan='4'>position</td>
            <th>s</th>
            <td>static</td>
        </tr>
        <tr>
            <th>r</th>
            <td>relative</td>
        </tr>
        <tr>
            <th>a</th>
            <td>absolute</td>
        </tr>
        <tr>
            <th>f</th>
            <td>fixed</td>
        </tr>
        <tr>
            <th>w</th>
            <td>width</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>h</th>
            <td>height</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>l</th>
            <td>left</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>r</th>
            <td>right</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>t</th>
            <td>top</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>b</th>
            <td>bottom</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>x</th>
            <td>left</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>y</th>
            <td>bottom</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>z</th>
            <td>z-index</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>pd</th>
            <td>padding</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>mg</th>
            <td>margin</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>pdt</th>
            <td>padding-top</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>mgt</th>
            <td>margin-top</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>pdb</th>
            <td>padding-bottom</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>mgb</th>
            <td>margin-bottom</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>pdl</th>
            <td>padding-left</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>mgl</th>
            <td>margin-left</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>pdr</th>
            <td>padding-right</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>mgr</th>
            <td>margin-right</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='2'>bs</th>
            <td rowspan='2'>box-sizing</td>
            <th>b</th>
            <td>border-box</td>
        </tr>
        <tr>
            <th>c</th>
            <td>content-box</td>
        </tr>
        <tr>
            <th rowspan='3'>fl</th>
            <td rowspan='3'>float</td>
            <th>l</th>
            <td>left</td>
        </tr>
        <tr>
            <th>r</th>
            <td>right</td>
        </tr>
        <tr>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th rowspan='3'>cl</th>
            <td rowspan='3'>clear</td>
            <th>l</th>
            <td>left</td>
        </tr>
        <tr>
            <th>r</th>
            <td>right</td>
        </tr>
        <tr>
            <th>b</th>
            <td>both</td>
        </tr>
        <tr>
            <th rowspan='5'>bi</th>
            <td rowspan='5'>break-inside</td>
            <th>n</th>
            <td>auto</td>
        </tr>
        <tr>
            <th>a</th>
            <td>avoid</td>
        </tr>
        <tr>
            <th>b</th>
            <td>always</td>
        </tr>
        <tr>
            <th>p</th>
            <td>avoid-page</td>
        </tr>
        <tr>
            <th>c</th>
            <td>avoid-column</td>
        </tr>
        <tr>
            <th rowspan='5'>pbb</th>
            <td rowspan='5'>page-break-before</td>
            <th>n</th>
            <td>auto</td>
        </tr>
        <tr>
            <th>a</th>
            <td>avoid</td>
        </tr>
        <tr>
            <th>b</th>
            <td>always</td>
        </tr>
        <tr>
            <th>p</th>
            <td>avoid-page</td>
        </tr>
        <tr>
            <th>c</th>
            <td>avoid-column</td>
        </tr>
        <tr>
            <th rowspan='5'>pbi</th>
            <td rowspan='5'>page-break-inside</td>
            <th>n</th>
            <td>auto</td>
        </tr>
        <tr>
            <th>a</th>
            <td>avoid</td>
        </tr>
        <tr>
            <th>b</th>
            <td>always</td>
        </tr>
        <tr>
            <th>p</th>
            <td>avoid-page</td>
        </tr>
        <tr>
            <th>c</th>
            <td>avoid-column</td>
        </tr>
        <tr>
            <th rowspan='5'>pba</th>
            <td rowspan='5'>page-break-after</td>
            <th>n</th>
            <td>auto</td>
        </tr>
        <tr>
            <th>a</th>
            <td>avoid</td>
        </tr>
        <tr>
            <th>b</th>
            <td>always</td>
        </tr>
        <tr>
            <th>p</th>
            <td>avoid-page</td>
        </tr>
        <tr>
            <th>c</th>
            <td>avoid-column</td>
        </tr>
        <tr>
            <th rowspan='4'>o</th>
            <td rowspan='4'>overflow</td>
            <th>v</th>
            <td>visible</td>
        </tr>
        <tr>
            <th>h</th>
            <td>hidden</td>
        </tr>
        <tr>
            <th>s</th>
            <td>scroll</td>
        </tr>
        <tr>
            <th>a</th>
            <td>auto</td>
        </tr>
        <tr>
            <th rowspan='4'>ox</th>
            <td rowspan='4'>overflow-x</td>
            <th>v</th>
            <td>visible</td>
        </tr>
        <tr>
            <th>h</th>
            <td>hidden</td>
        </tr>
        <tr>
            <th>s</th>
            <td>scroll</td>
        </tr>
        <tr>
            <th>a</th>
            <td>auto</td>
        </tr>
        <tr>
            <th rowspan='4'>oy</th>
            <td rowspan='4'>overflow-y</td>
            <th>v</th>
            <td>visible</td>
        </tr>
        <tr>
            <th>h</th>
            <td>hidden</td>
        </tr>
        <tr>
            <th>s</th>
            <td>scroll</td>
        </tr>
        <tr>
            <th>a</th>
            <td>auto</td>
        </tr>
        <tr>
            <th rowspan='6'>of</th>
            <td rowspan='6'>object-fit</td>
            <th>f</th>
            <td>fill</td>
        </tr>
        <tr>
            <th>c</th>
            <td>cover</td>
        </tr>
        <tr>
            <th>i</th>
            <td>contain</td>
        </tr>
        <tr>
            <th>cvr</th>
            <td>cover</td>
        </tr>
        <tr>
            <th>cnt</th>
            <td>contain</td>
        </tr>
        <tr>
            <th>sd</th>
            <td>scale-down</td>
        </tr>
        <tr>
            <th rowspan='1'>op</th>
            <td rowspan='1'>object-position</td>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th rowspan='4'>as</th>
            <td rowspan='4'>align-self</td>
            <th>f</th>
            <td>stretch</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>e</th>
            <td>end</td>
        </tr>
        <tr>
            <th>s</th>
            <td>start</td>
        </tr>
        <tr>
            <th>g</th>
            <td>grid-area</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>gr</th>
            <td>grid-row</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>gc</th>
            <td>grid-column</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>nth</th>
            <td>order</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## col

<table>
    <tbody>
        <tr>
            <th>c</th>
            <td>column-count</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>w</th>
            <td>column-width</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>g</th>
            <td>column-gap</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='10'>rs</th>
            <td rowspan='10'>column-rule-style</td>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th>h</th>
            <td>hidden</td>
        </tr>
        <tr>
            <th>s</th>
            <td>solid</td>
        </tr>
        <tr>
            <th>d</th>
            <td>dotted</td>
        </tr>
        <tr>
            <th>ds</th>
            <td>dashed</td>
        </tr>
        <tr>
            <th>w</th>
            <td>double</td>
        </tr>
        <tr>
            <th>r</th>
            <td>ridge</td>
        </tr>
        <tr>
            <th>g</th>
            <td>groove</td>
        </tr>
        <tr>
            <th>i</th>
            <td>inset</td>
        </tr>
        <tr>
            <th>o</th>
            <td>outset</td>
        </tr>
        <tr>
            <th>rw</th>
            <td>column-rule-width</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>rc</th>
            <td>column-rule-color</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## flx

<table>
    <tbody>
        <tr>
            <th rowspan='3'>w</th>
            <td rowspan='3'>flex-wrap</td>
            <th>n</th>
            <td>nowrap</td>
        </tr>
        <tr>
            <th>w</th>
            <td>wrap</td>
        </tr>
        <tr>
            <th>r</th>
            <td>wrap-reverse</td>
        </tr>
        <tr>
            <th rowspan='5'>jc|j</th>
            <td rowspan='5'>justify-content</td>
            <th>s</th>
            <td>flex-start</td>
        </tr>
        <tr>
            <th>e</th>
            <td>flex-end</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>b</th>
            <td>space-between</td>
        </tr>
        <tr>
            <th>a</th>
            <td>space-around</td>
        </tr>
        <tr>
            <th rowspan='5'>ac|v</th>
            <td rowspan='5'>align-content</td>
            <th>s</th>
            <td>flex-start</td>
        </tr>
        <tr>
            <th>e</th>
            <td>flex-end</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>b</th>
            <td>space-between</td>
        </tr>
        <tr>
            <th>a</th>
            <td>space-around</td>
        </tr>
        <tr>
            <th rowspan='5'>ji</th>
            <td rowspan='5'>justify-items</td>
            <th>s</th>
            <td>flex-start</td>
        </tr>
        <tr>
            <th>e</th>
            <td>flex-end</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>b</th>
            <td>space-between</td>
        </tr>
        <tr>
            <th>a</th>
            <td>space-around</td>
        </tr>
        <tr>
            <th rowspan='5'>ai|a</th>
            <td rowspan='5'>align-items</td>
            <th>s</th>
            <td>flex-start</td>
        </tr>
        <tr>
            <th>e</th>
            <td>flex-end</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>b</th>
            <td>baseline</td>
        </tr>
        <tr>
            <th>f</th>
            <td>stretch</td>
        </tr>
        <tr>
            <th rowspan='4'>d</th>
            <td rowspan='4'>flex-direction</td>
            <th>r</th>
            <td>row</td>
        </tr>
        <tr>
            <th>rr</th>
            <td>row-reverse</td>
        </tr>
        <tr>
            <th>c</th>
            <td>column</td>
        </tr>
        <tr>
            <th>cr</th>
            <td>column-reverse</td>
        </tr>
        <tr>
            <th>c</th>
            <td>列数均等化</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## grd

<table>
    <tbody>
        <tr>
            <th>t</th>
            <td>grid-template</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>rc</th>
            <td>grid-template-columns</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>rr</th>
            <td>grid-template-rows</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>tc</th>
            <td>grid-template-columns</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>tr</th>
            <td>grid-template-rows</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ac</th>
            <td>grid-auto-columns</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ar</th>
            <td>grid-auto-rows</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='3'>f</th>
            <td rowspan='3'>grid-auto-flow</td>
            <th>c</th>
            <td>column</td>
        </tr>
        <tr>
            <th>r</th>
            <td>row</td>
        </tr>
        <tr>
            <th>d</th>
            <td>dense</td>
        </tr>
        <tr>
            <th rowspan='6'>j</th>
            <td rowspan='6'>justify-content</td>
            <th>s</th>
            <td>start</td>
        </tr>
        <tr>
            <th>e</th>
            <td>end</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>b</th>
            <td>space-between</td>
        </tr>
        <tr>
            <th>a</th>
            <td>space-around</td>
        </tr>
        <tr>
            <th>v</th>
            <td>space-evenly</td>
        </tr>
        <tr>
            <th>a</th>
            <td>align-content</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ji</th>
            <td>justify-items</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ai</th>
            <td>align-items</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>g</th>
            <td>grid-gap</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## shd

<table>
    <tbody>
        <tr>
            <th rowspan='2'>b</th>
            <td rowspan='2'>box-shadow</td>
            <th>正数</th>
            <td>外側に上方光源の影</td>
        </tr>
        <tr>
            <th>負数</th>
            <td>内側に上方光源の影</td>
        </tr>
        <tr>
            <th rowspan='2'>bt</th>
            <td rowspan='2'>box-shadow</td>
            <th>正数</th>
            <td>要素上辺外側の影</td>
        </tr>
        <tr>
            <th>負数</th>
            <td>要素上辺内側の影</td>
        </tr>
        <tr>
            <th rowspan='2'>bb</th>
            <td rowspan='2'>box-shadow</td>
            <th>正数</th>
            <td>要素下辺外側の影</td>
        </tr>
        <tr>
            <th>負数</th>
            <td>要素下辺内側の影</td>
        </tr>
        <tr>
            <th rowspan='2'>bl</th>
            <td rowspan='2'>box-shadow</td>
            <th>正数</th>
            <td>要素左辺外側の影</td>
        </tr>
        <tr>
            <th>負数</th>
            <td>要素左辺内側の影</td>
        </tr>
        <tr>
            <th rowspan='2'>br</th>
            <td rowspan='2'>box-shadow</td>
            <th>正数</th>
            <td>要素右辺外側の影</td>
        </tr>
        <tr>
            <th>負数</th>
            <td>要素右辺内側の影</td>
        </tr>
        <tr>
            <th rowspan='1'>t</th>
            <td rowspan='1'>text-shadow</td>
            <th>数値</th>
            <td>上方光源の影</td>
        </tr>
    </tbody>
</table>


## svg

<table>
    <tbody>
        <tr>
            <th>f</th>
            <td>fill</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>s</th>
            <td>stroke</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>w</th>
            <td>stroke-width</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='3'>ta</th>
            <td rowspan='3'>text-anchor</td>
            <th>l</th>
            <td>start</td>
        </tr>
        <tr>
            <th>c</th>
            <td>middle</td>
        </tr>
        <tr>
            <th>r</th>
            <td>end</td>
        </tr>
        <tr>
            <th rowspan='3'>db</th>
            <td rowspan='3'>dominant-baseline</td>
            <th>t</th>
            <td>baseline</td>
        </tr>
        <tr>
            <th>m</th>
            <td>middle</td>
        </tr>
        <tr>
            <th>b</th>
            <td>hanging</td>
        </tr>
        <tr>
            <th rowspan='3'>e</th>
            <td rowspan='3'>stroke-linecap stroke-linejoin</td>
            <th>m</th>
            <td>square miter</td>
        </tr>
        <tr>
            <th>b</th>
            <td>butt bevel</td>
        </tr>
        <tr>
            <th>r</th>
            <td>round round</td>
        </tr>
        <tr>
            <th>d</th>
            <td>stroke-dasharray stroke-dashoffset</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## tbl

<table>
    <tbody>
        <tr>
            <th>自動</th>
            <td>sが空ならborder-collapse:collapse、指定されていればborder-collapse:separate</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>s</th>
            <td>border-spacing</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='2'>l</th>
            <td rowspan='2'>table-layout</td>
            <th>a</th>
            <td>auto</td>
        </tr>
        <tr>
            <th>f</th>
            <td>fixed</td>
        </tr>
        <tr>
            <th>r</th>
            <td>角丸</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## trn

<table>
    <tbody>
        <tr>
            <th>x</th>
            <td>translateX()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>y</th>
            <td>translateY()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>z</th>
            <td>translateZ()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>r</th>
            <td>rotateZ()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>rx</th>
            <td>rotateX()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ry</th>
            <td>rotateY()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>s</th>
            <td>scale()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>sx</th>
            <td>scaleX()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>sy</th>
            <td>scaleY()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>k</th>
            <td>skew()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>kx</th>
            <td>skewX()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ky</th>
            <td>skewY()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>hue</th>
            <td>hue-rotate()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>str</th>
            <td>saturate()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>brt</th>
            <td>brightness()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>inv</th>
            <td>invert()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>shd</th>
            <td>drop-shadow()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>blr</th>
            <td>blur()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>cnt</th>
            <td>contrast()</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>p</th>
            <td>perspective</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>d</th>
            <td>transition-delay</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>e</th>
            <td>transition-timing-function</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='8'>a</th>
            <td rowspan='8'>animation</td>
            <th>i</th>
            <td>infinite</td>
        </tr>
        <tr>
            <th>r</th>
            <td>reverse</td>
        </tr>
        <tr>
            <th>a</th>
            <td>alternate</td>
        </tr>
        <tr>
            <th>e</th>
            <td>ease</td>
        </tr>
        <tr>
            <th>l</th>
            <td>linear</td>
        </tr>
        <tr>
            <th>fw</th>
            <td>forwards</td>
        </tr>
        <tr>
            <th>bw</th>
            <td>backwards</td>
        </tr>
        <tr>
            <th>b</th>
            <td>both</td>
        </tr>
        <tr>
            <th>o</th>
            <td>opacity</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>t</th>
            <td>transition</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>tb</th>
            <td>順次トランジション</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='2'>bf</th>
            <td rowspan='2'>backface-visibility</td>
            <th>h</th>
            <td>hidden</td>
        </tr>
        <tr>
            <th>v</th>
            <td>visible</td>
        </tr>
        <tr>
            <th>to</th>
            <td>transform-origin</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


## txt

<table>
    <tbody>
        <tr>
            <th>i</th>
            <td>text-indent</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='5'>a</th>
            <td rowspan='5'>text-align</td>
            <th>l</th>
            <td>left</td>
        </tr>
        <tr>
            <th>r</th>
            <td>right</td>
        </tr>
        <tr>
            <th>c</th>
            <td>center</td>
        </tr>
        <tr>
            <th>j</th>
            <td>justify</td>
        </tr>
        <tr>
            <th>n</th>
            <td>nowrap</td>
        </tr>
        <tr>
            <th>h</th>
            <td>line-height</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='4'>v</th>
            <td rowspan='4'>vertical-align</td>
            <th>t</th>
            <td>top</td>
        </tr>
        <tr>
            <th>m</th>
            <td>middle</td>
        </tr>
        <tr>
            <th>b</th>
            <td>bottom</td>
        </tr>
        <tr>
            <th>l</th>
            <td>baseline</td>
        </tr>
        <tr>
            <th>f</th>
            <td>font-family</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>p</th>
            <td>font-size</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>t</th>
            <td>letter-spacing</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>ls</th>
            <td>letter-spacing</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>c</th>
            <td>color</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='8'>s</th>
            <td rowspan='8'>font-weight|font-style|text-decoration</td>
            <th>r</th>
            <td>normal</td>
        </tr>
        <tr>
            <th>b</th>
            <td>bold</td>
        </tr>
        <tr>
            <th>l</th>
            <td>lighter</td>
        </tr>
        <tr>
            <th>i</th>
            <td>italic</td>
        </tr>
        <tr>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th>u</th>
            <td>underline</td>
        </tr>
        <tr>
            <th>o</th>
            <td>overline</td>
        </tr>
        <tr>
            <th>s</th>
            <td>line-through</td>
        </tr>
        <tr>
            <th rowspan='9'>w</th>
            <td rowspan='9'>font-weight</td>
            <th>t</th>
            <td>100</td>
        </tr>
        <tr>
            <th>e</th>
            <td>200</td>
        </tr>
        <tr>
            <th>l</th>
            <td>300</td>
        </tr>
        <tr>
            <th>r</th>
            <td>400</td>
        </tr>
        <tr>
            <th>m</th>
            <td>500</td>
        </tr>
        <tr>
            <th>d</th>
            <td>600</td>
        </tr>
        <tr>
            <th>b</th>
            <td>700</td>
        </tr>
        <tr>
            <th>u</th>
            <td>800</td>
        </tr>
        <tr>
            <th>h</th>
            <td>900</td>
        </tr>
        <tr>
            <th>fw</th>
            <td>font-weight</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>fs</th>
            <td>font-style</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>td</th>
            <td>text-decoration</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='3'>to</th>
            <td rowspan='3'>text-oriantation</td>
            <th>m</th>
            <td>mixed</td>
        </tr>
        <tr>
            <th>s</th>
            <td>sideway</td>
        </tr>
        <tr>
            <th>u</th>
            <td>upright</td>
        </tr>
        <tr>
            <th rowspan='8'>l</th>
            <td rowspan='8'>list-style</td>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th>ds</th>
            <td>disc</td>
        </tr>
        <tr>
            <th>cr</th>
            <td>circle</td>
        </tr>
        <tr>
            <th>sq</th>
            <td>square</td>
        </tr>
        <tr>
            <th>alp</th>
            <td>upper-alpha</td>
        </tr>
        <tr>
            <th>dec</th>
            <td>decimal</td>
        </tr>
        <tr>
            <th>rom</th>
            <td>upper-roman</td>
        </tr>
        <tr>
            <th>hira</th>
            <td>hiragana</td>
        </tr>
        <tr>
            <th>whs</th>
            <td>white-space</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>wds</th>
            <td>word-spacing</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>wb</th>
            <td>word-break</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th rowspan='3'>b</th>
            <td rowspan='3'>word-break</td>
            <th>k</th>
            <td>keep-all</td>
        </tr>
        <tr>
            <th>b</th>
            <td>break-all</td>
        </tr>
        <tr>
            <th>n</th>
            <td>normal</td>
        </tr>
        <tr>
            <th rowspan='3'>ffs</th>
            <td rowspan='3'>font-feature-settings</td>
            <th>p</th>
            <td>"palt"</td>
        </tr>
        <tr>
            <th>t</th>
            <td>"trad"</td>
        </tr>
        <tr>
            <th>n</th>
            <td>"nalt"</td>
        </tr>
        <tr>
            <th rowspan='3'>m</th>
            <td rowspan='3'>writing-mode</td>
            <th>h</th>
            <td>horizontal-tb</td>
        </tr>
        <tr>
            <th>vr</th>
            <td>vertical-rl</td>
        </tr>
        <tr>
            <th>vl</th>
            <td>vertical-lr</td>
        </tr>
    </tbody>
</table>


## usr

<table>
    <tbody>
        <tr>
            <th rowspan='2'>c</th>
            <td rowspan='2'>cursor</td>
            <th>p</th>
            <td>pointer</td>
        </tr>
        <tr>
            <th>w</th>
            <td>wait</td>
        </tr>
        <tr>
            <th rowspan='2'>e</th>
            <td rowspan='2'>pointer-events</td>
            <th>a</th>
            <td>auto</td>
        </tr>
        <tr>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th rowspan='4'>s</th>
            <td rowspan='4'>user-select</td>
            <th>n</th>
            <td>none</td>
        </tr>
        <tr>
            <th>a</th>
            <td>all</td>
        </tr>
        <tr>
            <th>t</th>
            <td>text</td>
        </tr>
        <tr>
            <th>c</th>
            <td>contain</td>
        </tr>
    </tbody>
</table>


