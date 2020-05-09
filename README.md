var marked = require('marked');
var renderer = new marked.Renderer();

renderer.heading = function (text, level) {
  var escapedText = text.toLowerCase().replace(/[^\w]+/g, '-');

  return '<h' + level + '><a name="' +
                escapedText +
                 '" class="anchor" href="#' +
                 escapedText +
                 '"><span class="header-link"></span></a>' +
                  text + '</h' + level + '>';
},

console.log(marked('# heading+', { renderer: renderer }));

# glowing-giggle

#work in progress




<svg viewBox="0 0 20 10" xmlns="http://www.w3.org/2000/svg">
  <circle cx="5" cy="5" r="4">
    <title>I'm a circle</title>
  </circle>

  <rect x="11" y="1" width="8" height="8">
    <title>I'm a square</title>
  </rect>
</svg>



You need to open the [image](//raw.githubusercontent.com/htonchia/glowing-giggle/master/dens_surhosmarcom92_.svg) in your browser to read the commune name by pointing it with the mouse.


![](dens_surhosmarcom92_.svg)


![](svg_histogram.svg)

<img style="float: right;" src="dens_surhosmarcom92_.svg">
