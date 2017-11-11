# flexbox-cheatsheet
Cheatsheet to reference for flexbox values

Based on going through [flexboxfroggy.com](http://flexboxfroggy.com/)
```

Element with 
  .element { display: flex; }
    can have the following properties:

Horizontal alignment (unless you apply flex-direction: columnn, then verticle)
  {
    justify-content: 
      flex-start:    Items align to the left side of the container.
      flex-end:      Items align to the right side of the container.
      center:        Items align at the center of the container.
      space-between: Items display with equal spacing between them.
      space-around:  Items display with equal spacing around them.
  }

Verticle alignment (unless you apply flex-direction: columnn, then horizontal)
  {
    align-items:
      flex-start: Items align to the top of the container.
      flex-end:   Items align to the bottom of the container.
      center:     Items align at the vertical center of the container.
      baseline:   Items display at the baseline of the container.
      stretch:    Items are stretched to fit the container.
  }

Horizontal / Verticle Direction
  {
    flex-direction:
      row:            Items are placed the same as the text direction.
      row-reverse:    Items are placed opposite to the text direction.
      column:         Items are placed top to bottom.
      column-reverse: Items are placed bottom to top.
  }

Order items:
  Items in a flex container have a order given to them automatically, 
  ...-1, 0, 1, 2... etc and you can set these items order by using
  {
    order: 2; (or whatever number)
  }

Target specific element:
  Can target a specific .element(s) { } using align-self, so you don't need
    to apply alignment attributes to everything within the container, 
    but can target them with a class.

  {
    align-self: <see all options for align-items>
  }

Wrapping items:
  {
    flex-wrap:
      nowrap:       Every item is fit to a single line.
      wrap:         Items wrap around to additional lines.
      wrap-reverse: Items wrap around to additional lines in reverse.
  }

Shorthand for using flex-direction with flex-wrap
  flex-flow is a shorthand for flex-direction and flex-wrap.
    Just makes it so you can put them both on the same line instead of 
    having to declare both.

  {
    flex-flow: <flex-direction> <flex-wrap>
  }

Declare how multiple lines  of content should be spaced
  {
    align-content:
      flex-start:    Lines are packed at the top of the container.
      flex-end:      Lines are packed at the bottom of the container.
      center:        Lines are packed at the vertical center of the container.
      space-between: Lines display with equal spacing between them.
      space-around:  Lines display with equal spacing around them.
      stretch:       Lines are stretched to fit the container.
  }
```
