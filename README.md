# NASA - Event Page

## [ViewSite](http://gabdong.dothome.co.kr/nasa)

***

NASA의 이벤트 페이지를 제작하였습니다.
jQuery를 이용하여 배경화면 조작이 가능한 이벤트페이지입니다.

***

## nasa_index.js

```javascript
$('figure>video').next().css({
	'right':'540px'
});
$('figure>video').next().next().css({
	'right':'470px'
});
$('figure>video').next().next().next().css({
	'right':'400px'
});
$('button').css({
	'border':'none',
	'background':'none',
	'cursor':'pointer',
	'position':'absolute',
	'top':'50px'
});
$('button>i').css({
	'font-size':'30px',
	'color':'#fff'
});

//동영상 제어
$('figure button').eq(0).click(function(){
	/*get():선택한 요소를 배열로 가져오는 메서드*/
	$('figure').find('video').get(0).play();
});
$('figure button').eq(1).click(function(){
	$('figure').find('video').get(0).pause();
});
$('figure button').eq(2).click(function(){
	$('figure').find('video').get(0).load();
});
```
