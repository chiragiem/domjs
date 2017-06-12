
# domjs
Create HTML script easily and faster with lesser code and complexity

<h1>Introduction</h1>
Creating fron-end app, with JS script rendering all your HTML could become complex and messier as your project grows. Embedding HTML script directly into JS script make it difficult to write and maintain code. Also Dom method requires lot of steps, to accompalish the same task. Hence this library aims to reduce pain of front-end developers.

<h1>Set up</h1>
Add this code inside "head" element to access the library.
<code><script src="js/Dom.js" type='text/javascript'></script></code>

<h1>Syntax</h1>
<hr>
<h3>domElement(tag,attributes,styles,param)</h3>
This constructor should be passed 4 argumments
<ul>
<li>'tag'- string containing tag name of the element/node to create</li>
<li>attributes[object] - Object containing attributes, to assign to element/node to be created. Attribute name and its value will be the property name and value </li>
<li>style[object]- Object containing css properties, to assign to element/node to be created. style name and its value will be the property name and value </li>
<li>param - This fourth argument is either String or an already created element/node object. This argument tells whether new element is to be created or already created element should be appended as child to new element being created</li>
</ul>
<h1>Use</h1>
<h3>Creating new Element</h3>

<code>var attr = {
  class:"col-xs-12 superhero",
  id:"iron-man"
 }
 </code>
 
<code>
var sty = {
  backgroundColor:"white",
  borderRadius:"3px"
 }
</code>
<br>
 
<code> var elem = new domElement("h3",attr,sty,"Iron Man");</code>

Notice, here 4th argument is String.

<h3>Appending to creating element/node already existing element/node</h3>
<code>var box1 = new domElement("div",{class:"row"},{marginTop:"15px"},elem)</code>

Notice, here last argument is element/node object already created

<h3>Contribution</h3>
Contribute to this project, to improve this library and make it even more powerfull
