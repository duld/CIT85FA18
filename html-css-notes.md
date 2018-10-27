# HTML and CSS notes

## CSS Combinators

### Adjacent Sibling Combinator +

* seperates two selectors and matches the second element
* the match only takes place if the second element immediately
  follows the first element.

```CSS

div + p {
  background-color: blue;
}

```

### Descendant Combinator ' '

* Typically represented by a single space character
* combines two selectors such that elements matched by the second
  selector are selected if they have an ancestor element matching
  the first selector.
* Selectors that utilize a descendant combinator are called descendant
  selectors.

```CSS

div p {
  background-color: blue;
}

```

### General Sibling Combinator ~

* Seperates two selectors and matches the second element only if it
  follows the first element.

```CSS

div ~ p {
  background-color: blue;

}

```

### Child Combinator >

* Placed between two CSS selectors
* Matches only those elements matched by the second selector that are
  the children of elements matched by the first.

```CSS

div > p {
  background-color: blue;

}

```

## Box Model

Everything on the web is a box. The box is made up of:

* Content
* Padding
* Border
* Margin

### Box-Sizing

The Box-Sizing attribute declares how the width and height you assign to an HTML element is applied. By default the height/width is applied to the content (content-box). Border-Box applies the width and height to the content, padding and border.

#### Border-Box

The __width__ and __height__ properties include the content, padding, and th border, but do not include the margin. Note that the padding and border will be inside the box.

#### Content-Box

This is th einitial and default value as specified byt he CSS standard. The width and height properties include the content, but does not include the padding, border, or margin.