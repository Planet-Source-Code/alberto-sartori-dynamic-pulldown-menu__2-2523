<div align="center">

## Dynamic pulldown menu


</div>

### Description

When you choose an item from the first menu, it appears related items in the seconds.
 
### More Info
 
You can customize the menu items as you want.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alberto Sartori](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alberto-sartori.md)
**Level**          |Intermediate
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |
**Category**       |[Controls/ Forms/ Graphics/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-graphics-menus__2-59.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alberto-sartori-dynamic-pulldown-menu__2-2523/archive/master.zip)





### Source Code

```

<HTML>
<HEAD>
<TITLE></TITLE>
<script language = "JavaScript">
<!--
var names = new Array("Mark","Sarah","Carl","James");
var fruit = new Array("Banana","Strawberry","Apple");
var colors = new Array("Red", "White", "Green", "Brown");
function swapOptions(the_array_name)
{
    var numbers_select = window.document.myform.examples;
    var the_array = eval(the_array_name);
    setOptionText(window.document.myform.examples,the_array);
}
function setOptionText(the_select, the_array)
{
		the_select.length=the_array.length;
    for (c=0; c < the_array.length; c++)
    {
        the_select.options[c].text = the_array[c];
    }
}
//-->
</script>
</HEAD>
<form name="myform">
<select size="1" name="category" onChange="swapOptions(window.document.myform.category.options[selectedIndex].text);">
<option>names
<option>fruit
<option>colors
</select>
<select size="1" name="examples">
<option>-------
</select>
</form>
</body>
</html>
```

