```ele``` key is used to refer to html tag

In order to create a ```div``` element
```
{ 
  ele : 'div',
}
```

``` attr ``` key is used to refer to attributes of html tag except style attribute

In order to gave the above div element class of `class` ( use space to separate multiple classname e.g. 'classes another' and id of `id`

```
{
   ele : 'div',
   attr : {
     id : 'id',
     class : 'classes'
   },
}

```

``` style ``` key is used to refer to the style of html tag

use camelcasing for style keys, e.g. font-style === fontStyle, text-align === textAlign and so on.

```

{
   ele : 'div',
   attr : {
     id : 'id',
     class : 'classes'
   },
   style : {
     color : 'red',
     backgroundColor: 'black',
   }
}

```

```child``` key is used to create childs of the html tag, its contains array of objects as value, each object within that array contains same object as above

```

{
   ele : 'div',
   attr : {
     id : 'id',
     class : 'classes'
   },
   style : {
     color : 'red',
     backgroundColor: 'black',
   },
   child: [
       {
         ele : 'p',
         attr : {
            id : 'p_child',         
         }
       },
       {
         ele : 'p',
         attr : {
            id : 'p_child_2',         
         }
       },
       
       
   ]
}

```

```text``` key to add text to element

```

{
   ele : 'div',
   attr : {
     id : 'id',
     class : 'classes'
   },
   style : {
     color : 'red',
     backgroundColor: 'black',
   },
   child: [
       {
         ele : 'p',
         attr : {
            id : 'p_child',         
         },
         text: 'This is first p',
       },
       {
         ele : 'p',
         attr : {
            id : 'p_child_2',         
         },
         text: 'This is second p',
       },
       
       
   ]
}

```

# Result of above code

```
<div class="classes" id="id">
  <p id="p_child">This is first p</p>
  <p id="p_child_2">This is second p</p>
</div>
```


# Project

{
   'id of the method` : {
       object for the id
   }
}

```
{
   md5 : {
      ele : 'div',
      attr : {...},
      child : [ {...}, {...}],
   }

}

```
