# css3 transform on browser scroll



브라우저를 수직으로 스크롤하면서, 상단 곡선이미지가 자연스럽게 축소되는 것처럼 보이게 한다.

>```javascript
>var curve_scroll = document.querySelector('.curve')
>
>window.addEventListener('scroll', function(){
>    var value = 1 + window.scrollY/-500;
>    curve_scroll.style.transform = `scaleY(${value})`
>})
>```