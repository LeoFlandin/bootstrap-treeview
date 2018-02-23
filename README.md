# Bootstrap Tree View Leo's Patch

---

Original repo : [/bootstrap-treeview](https://github.com/jonmiles/bootstrap-treeview/)


### Usage

The object of this fork is to add the hability to dynamically render the text node by passing a function.
The function is called with the node object. 

Example

```javascript
var tree = [
    {
    text: function(node){
      return new Date() + "Node #" + node.nodeId + " Business : " + node.myBusinessData; 
    },
    myBusinessData: "foobar"
];
```
The function is evaluated in each ``render`` process, including node click, node select, node collapse, etc.
 

