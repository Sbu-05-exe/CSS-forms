# Notes :writing:

The `~` CSS selector operand is used to select sibling elements. But it seems to only select sibling elements that before the element that is referenced

i.e. 

```HTML
 <span></span>
 <input type="" name="">
```
you can use the selector `input ~ span` to select the span element but you can't use `span ~ input` to select the input element

###CSS tricks


The tick was created by using a 2 sides of a border of a span:after element

The position of absolute elements are relative to the body unless. You can override this by making a container have a position of `relative` and all its child elements with a position of `absolute` will be positioned relative to the container. Position `absolute` will make other elements ignore other elements positions so they can overlap and stuff.