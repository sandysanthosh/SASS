Welcome to the SASS wiki!


sass:

* Sass is the most mature, stable, and powerful professional grade CSS extension language in the world.

* shorthand version


* ->scss:


`<link rel="stylesheet" type="text/css" href="main.scss">`

* ->style awesome stylesheet

* ->ruby installer

* install sass:
* css compiler
* regular css


* ->nesting
* ->partials
* ->mixins
* ->extend,inherited

### main.css:

`$primary-color: green;`
`$ff: #f2f2f2;`
`$bg: red;`

`@import 'colors';`
`@import 'mixins';`

`body{`
`background: $bg;`
`font-family: $ff;`
`}`
`h1{`
`color:$primary-color;`
`}`
`p`
`{ `
`color:$primary-color;`
`}`

`.container{`
`ul li{`
 `padding: 10px;`
`}`
`#box{`
`backgroung:red;`
`@include border-radius(5px);}`
`height:20px;`
`width:20px;`
`}`


### index.html:

`<div class="container">`
`<div id="box">`
`<p>test</p>`
`<p>test11</p>`
`</div>`
`<h2>list</h2>`
`<ul>`
`<li>dog</li>`
`<li>cat</li>`
`<li>cat</li>`
`</ul>`
`</div>`
`</body>`
`</html>`


### color.scss:

`.blue{color:'blue';}`
`.red{color:'red';}    //partials`


### mixins.scss:

`@mixin border-radius($radius) {                  //boder radius`
  `-webkit-border-radius: $radius; `
     `-moz-border-radius: $radius;`
      `-ms-border-radius: $radius;`
          `border-radius: $radius;`
`}`

`.box { @include border-radius(10px); }`




