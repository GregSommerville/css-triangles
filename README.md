# css-triangles
Shows how to draw triangles using CSS

## Overview
CSS3 is a powerful system for formatting HTML elements, but sometimes it feels a little limiting when you want to do something that isn't strictly rectangular.  Sure, you can make a DIV tag have rounded corners with the `border-radius` attribute, but ultimately HTML and CSS are focused on blocks, and those blocks are rectangular.

Because of that, most triangles are rendered using image files or scalable vector graphics (SVG).  However, you can use pure CSS to create triangles of all sizes and shapes.  Let's look at how to accomplish that.

## It's All About the Borders
The `border-width` attribute of a DIV specifies the width of the border, obviously.  Setting that attribute will specify the width to be used on the left, right, top and bottom borders - it's shorthand for specifying each of those four attributes at once. But of course each of the four borders can have an individual width and color, which is the key to creating triangles.

Let's look at an example of a DIV with a very large border.  We'll color each of the four sides of the border a different color, so you can see how each border is drawn.

```
<style>
  .demo {
    width: 500px;
    height: 400px;
    border-width: 50px;
    border-top-color: green;
    border-bottom-color: green;
    border-left-color: blue;
    border-right-color: blue;
  }
</style>
<div class='demo'></div>
```

The above code results in this:

Notice how the edges between the border sides are bevelled.  

![beveled border edges](img/border-bevel.png)



## Authors
* **Greg Sommerville** - *Initial work* 
 
## License
This project is licensed under the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details