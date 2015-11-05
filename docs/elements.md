# Elements

Elements are things inside your component.

![](images/component-elements.png)

## Naming elements
Each component may have elements.

The elements are separated from the components with a dash.
They can be named with **one or more words**, separated by an __underscore__.

```scss
.component { /* ... */ } // component
.component-element { /* ... */ } // element
.component_name-element_name { /* ... */ } // more words
.component_name-another_element { /* ... */ } // more words
```

```scss
.field_action { /* ... */ } // component
.field_action-input { /* ... */ } // element
.field_action-button-search { /* ... */ } // element
```

## Element selectors
Try not to nest your css selectors.
Just because you can in scss, doesn't mean you should.

From the [sass-lang](http://sass-lang.com/guide) site:
> Be aware that overly nested rules will result in over-qualified CSS that could prove hard to maintain and is generally considered bad practice.

**Don't do this:**

```scss
.article-card {
  > .author  { /*  bad */ }
  .title  { /* worst */ }
}
```

> Question:

> You cant change the original css, how do you change the .title font-size?

> ```css
> .article-card.author .title  { /* */ }
> ```

> And if the css was like this?

> ```css
> .article_card-title  { /* */ }
> ```
> **Better, right?**


With legacy code this happens all the time!


## Avoid tag selectors
Use classes whenever possible.

Not for performance or whatever others say.

Its about maintainability! Always!

How many times you have to change a h2 to h3? Or span to a, or ul,li to div, p and vice-versa.

----

Not all elements should always look the same. Variants can help.
[Continue →](variants.md)
<!-- {p:.pull-box} -->
