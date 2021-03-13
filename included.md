---
layout: spectre
title: Simple Discovery Workflow
permalink: /included/
---

<p align="center"><iframe width="100%" height="100%" src="https://immunedynamics.io/Untitled" frameborder="0" style="border:1px solid black" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

<br />
<br />
<br />

<p align="center"><iframe width="100%" height="600" src="/pdfs/discovery.pdf" frameborder="0" style="border:1px solid black" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

<br />
<br />
<br />

<script>
function includeHTML() {
  var z, i, elmnt, file, xhttp;
  /* Loop through a collection of all HTML elements: */
  z = document.getElementsByTagName("*");
  for (i = 0; i < z.length; i++) {
    elmnt = z[i];
    /*search for elements with a certain atrribute:*/
    file = elmnt.getAttribute("w3-include-html");
    if (file) {
      /* Make an HTTP request using the attribute value as the file name: */
      xhttp = new XMLHttpRequest();
      xhttp.onreadystatechange = function() {
        if (this.readyState == 4) {
          if (this.status == 200) {elmnt.innerHTML = this.responseText;}
          if (this.status == 404) {elmnt.innerHTML = "Page not found.";}
          /* Remove the attribute, and call this function once more: */
          elmnt.removeAttribute("w3-include-html");
          includeHTML();
        }
      }
      xhttp.open("GET", file, true);
      xhttp.send();
      /* Exit the function: */
      return;
    }
  }
}
</script>
  
<!--<div w3-include-html="https://immunedynamics.io/markdown3"></div>-->
<div w3-include-html="markdown4.html"></div>
<div w3-include-html="/markdown4.html"></div>

<script>
includeHTML();
</script>

<br />
<br />
<br />
