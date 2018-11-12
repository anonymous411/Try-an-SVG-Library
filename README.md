# Try-an-SVG-Library

<title>SVG.js TextPath</title>
<meta http-equiv="content-type" content="text/html; charset=UTF-8">
<meta name="robots" content="noindex, nofollow">
<meta name="googlebot" content="noindex, nofollow">
<meta name="viewport" content="width=device-width, initial-scale=1">


<script type="text/javascript" src="/js/lib/dummy.js"></script>

  <link rel="stylesheet" type="text/css" href="/css/result-light.css">

    <script type="text/javascript" src="https://cdn.rawgit.com/svgdotjs/svg.js/ceaf24d5/dist/svg.min.js">
</script>


<style type="text/css">
  @import url('https://fonts.googleapis.com/css?family=Inconsolata');
#drawing {
width: 100%;
height: 300px;
}
tspan {
fill: #e5e5e5;
stroke: #f06;
stroke-width: 0.85;
font-family: 'Inconsolata';
}
input[type=text] {
width: 100%;
font-family: 'Inconsolata';
font-size: 14px;
outline: none;
color: #666;
}
</style>
<!-- TODO: Missing CoffeeScript 2 -->

<script type="text/javascript">


      window.onload=function(){

  var input = document.querySelector('input[type=text]')
  var draw = SVG('drawing').viewbox(0, 0, 300, 140)
  var text = draw.text(function(add) {
    add.tspan( input.value )
  })

  text
    .path('M10 80 C 40 10, 65 10, 95 80 S 150 150, 180 80')
    .animate(1000, '<>')
    .plot('M10 80 C 40 150, 65 150, 95 80 S 150 10, 180 80')
    .loop(true, true)

  input.addEventListener('keyup', updateText(text))

  function updateText(textPath) {
    return function() {
      textPath.tspan(this.value)
    }
  }
      }
</script>
</head>


<body>
<input type="text" value="Dragon----- - - - ->" placeholder="Type text here...">
<div id="drawing"><svg id="SvgjsSvg1006" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" id="SvgjsPath1011" d="M10 80C40 149.70968908436308 65 149.70968908436308 95 80S150 10.290310915636923 180 80 "></path></defs><text id="SvgjsText1008" font-family="Helvetica, Arial, sans-serif"><textPath id="SvgjsTextPath1010" xlink:href="#SvgjsPath1011"></tspan></textPath></text></svg></div>

<script>
  // tell the embed parent frame the height of the content
  if (window.parent && window.parent.parent){
    window.parent.parent.postMessage(["resultsFrame", {
      height: document.body.getBoundingClientRect().height,
      slug: "7wL1uv8n"
    }], "*")
  }
</script>


<svg id="SvgjsSvg1001" width="2" height="0" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:svgjs="http://svgjs.com/svgjs" style="opacity: 0; position: fixed; left: 100%; top: 100%; overflow: hidden;"><defs id="SvgjsDefs1002"></defs><polyline id="SvgjsPolyline1003" points="0,0"></polyline><path id="SvgjsPath1004" d="M0 0 "></path></svg></body></html>









<script>
var input = document.querySelector('input[type=text]')
var draw = SVG('drawing').viewbox(0, 0, 300, 140)
var text = draw.text(function(add) {
add.tspan( input.value )
})

text
.path('M10 80 C 40 10, 65 10, 95 80 S 150 150, 180 80')
.animate(1000, '<>')
.plot('M10 80 C 40 150, 65 150, 95 80 S 150 10, 180 80')
.loop(true, true)

input.addEventListener('keyup', updateText(text))

function updateText(textPath) {
return function() {
  textPath.tspan(this.value)
}
}
</script>


