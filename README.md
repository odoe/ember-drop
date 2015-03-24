# Ember-Drop

Ember-Drop is an Ember addon that wraps the [Drop.js](https://github.com/HubSpot/drop) library.

It is mostly just a wrapper, but does provide a few extra features, to make common tasks easier.

## Getting started

To start, if you are using Ember CLI, simply run:
```bash
ember install:addon ember-drop
```

After installing, just include the component in the template for the page you would like to attach the drop to.

```hbs
{{ember-drop
classes='drop-theme-arrows-bounce-dark'
content=hoverContent
openOn='hover'
position='top center'
targetSelector='.hover-element'}}
```

### classes
**classes** are extra classes to add to the drop. You'll want to add classes here for themes, if you are using them.

### content
**content** is an array of objects that denote the text, buttons, events, etc. that you want in your drop

### openOn
**openOn** is one of the following strings 'hover', 'click' or 'always'. These are pretty self explanatory.

### position
**position** is a string denoting the positioning of the drop, relative to the target it's attached to.

Possible options:
```

'top left'

'left top'

'left middle'

'left bottom'

'bottom left'

'bottom center'

'bottom right'

'right bottom'

'right middle'

'right top'

'top right'

'top center'

```

### targetSelector
**targetSelector** is the css selector of the element you want to attach the drop to.
