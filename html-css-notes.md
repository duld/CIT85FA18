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
