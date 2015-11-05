Components
==========

Think in components. Consider of each piece of your UI as an individual "component."

![](images/component-example.png)

A component can have another components inside.

Don't be afraid of building components that uses many other components.

## Naming components

>

Components can be named with **one or more words**, separated by an __underscore__.

Examples of a component:

  * A component (`.component`)
  * A component with more words (`.component_multi_words`)
  * A generic button (`.button`)
  * A form (`.form`)
  * A product feature (`.product_feature`)
  * A breadcrumb (`.breadcrumb`)
  * A section title (`.section_title`)
  * A menu hamburger (`.aside_menu`) _in this case the hamburger is just a
   component inside the menu_

> Why underscores? The other frameworks use dashes!

> It's easier to edit, with **one** _"Alt + →"_ you select the full component.

> Select a `.component-name` and a `.component_name` to see the difference.

>> Smart people sometimes don't think about the small things.

Components are the main classes in the css, it should be the easiest to write
 and edit.

How do you write a component exactly? Let's learn about Elements.
[Continue →](elements.md)
<!-- {p:.pull-box} -->
