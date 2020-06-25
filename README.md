# cawpow-scss

catpow-scssはscssのコードを短く手早く書くことを目的としたmixin集です。
catpow-scssはmixinは2〜3文字の短い名前で、複数のプロパティを同じく2〜3文字の短い名前で指定して設定できます。

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
