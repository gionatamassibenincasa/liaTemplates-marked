<!--
author:   Gionata Massi

email:    gionata.massi@gmail.com

version:  0.0.1

language: en

narrator: US English Female

comment:  Just a simple Marked template for LiaScript.

script:   https://cdn.jsdelivr.net/npm/marked/marked.min.js


@Markdown.eval: @Markdown._eval_(@uid)

@Markdown._eval_
<script>
let container = document.getElementById('marked-container-@0');

let out = marked(`@input`);

container.innerHTML = out;

"LIA: stop"
</script>

<div id="marked-container-@0" class="container"></div>

<script>
console.log("Inizializzazione");
let rem = document.getElementsByClassName("container")

for( let i=0; i< rem.length; i++ )
  rem[i].innerHTML = ""

console.log("delete content")
</script>
@end


-->


# Marked - Template


```md
# Titolo
```
@Markdown.eval
