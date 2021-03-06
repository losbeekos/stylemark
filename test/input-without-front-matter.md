A button can be used with `<button>` and `<a>` elements.

```html
<a class="btn btn-default" href="#">Button</a>
<button class="btn btn-default">Button</button>
```


Types
-----
Buttons can have several types:

class | description
--- | ---
`btn-default` | Standard button
`btn-primary` | Primary call-to-action
`btn-success` | Indicates a successful or positive action

```types.html
<button class="btn btn-default">Default</button>
<button class="btn btn-primary">Primary</button>
<button class="btn btn-success">Success</button>
```
```types.css hidden
button { margin: 5px; }
```
```types.js hidden
$('button').click(function() { alert('Button clicked!'); });
```


Sizes
-----
Buttons have different sizes available:
- `btn-sm`
- `btn-lg`

```sizes.html hidden height=100
<button class="btn btn-default btn-sm">Small</button>
<button class="btn btn-default">Default</button>
<button class="btn btn-default btn-lg">Large</button>
```


Frameworks
----------
Buttons can be used with Handlebars, React/JSX, and AngularJS.

In Handlebars:
```handlebars-button.handlebars
{{#bs-button}}Button{{/bs-button}}
```

In React/JSX:
```react-button.jsx
<Button>Button</Button>
```

In AngularJS:
```angular-button.html
<button class="btn btn-default">{{ text }}</button>
```
```angular-button.angularjs
text = 'Button'
```


Edge cases
----------
Pipes (`|`) can be escaped in tables:

One | Two | Three
--- | --- | ---
foo | an escaped pipe \| lives here | bar
what | `{{ 'foo' \| bar }}` | who

< and > can also be escaped to prevent them from being treated as HTML tags: \<foo\>


Disabled state
--------------
Buttons can be disabled too.

```disabled.html
<button class="btn btn-primary" disabled>Disabled button</button>
```
