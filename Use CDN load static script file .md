```js
<script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="js/jquery-1.11.0.min.js" type="text/javascript"><\/script>')</script>
// or

<script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script>if(typeof jQuery =="undefined"){
        var head = document.getElementsByTagName('head')[0];
        var script = document.createElement('script');
        script.src = "js/jquery-1.11.0.min.js";
        script.type = 'text/javascript';
        head.appendChild(script);
}</script>
```
