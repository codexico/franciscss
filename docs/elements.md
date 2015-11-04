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
Prefer to use the `>` child selector whenever possible. This prevents bleeding through nested components, and performs better than descendant selectors.

```scss
.article-card {
  .title     { /* okay */ }
  > .author  { /* ✓ better */ }
}
```

## On multiple words
For those that need two or more words, concatenate them without dashes or underscores.

```scss
.profile-box {
  > .firstname { /* ... */ }
  > .lastname { /* ... */ }
  > .avatar { /* ... */ }
}
```

## Avoid tag selectors
Use classnames whenever possible. Tag selectors are fine, but they may come at a small performance penalty and may not be as descriptive.

```scss
.article-card {
  > h3    { /* ✗ avoid */ }
  > .name { /* ✓ better */ }
}
```

Not all elements should always look the same. Variants can help.
[Continue →](variants.md)
<!-- {p:.pull-box} -->
