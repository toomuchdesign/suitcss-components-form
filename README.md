# SUIT CSS components-form

[![Build Status](https://travis-ci.org/toomuchdesign/suitcss-components-form.svg?branch=master)](https://travis-ci.org/toomuchdesign/suitcss-components-form)

A very lightweight SUIT component for forms.

Read more about [SUIT's design principles](https://github.com/suitcss/suit/).

For a more extended approach see giuseppeg's [suitcss-components-form](https://github.com/giuseppeg/suitcss-components-form).

This library is a mantainance fork of an [old draft](https://github.com/trunkclub/suitcss-components-form) by [Nicolas Gallagher](https://github.com/necolas).


## Installation

- [NPM](http://www.npmjs.com/): `npm install @toomuchdesign/suitcss-components-form --save`
- Download: [zip](https://github.com/toomuchdesign/suitcss-components-form/releases/latest)


## Available classes

- `Form` - Provides some basic display and alignment adjustments to form elements.
- `Form--inline` -.
- `Form-field` - The wrapper for a label-control pair.
- `Form-field--stacked` - Modifier to stack labels on top of controls.
- `Form-label` - A control's _visual_ label.
- `Form-input` - Styles intended for text-based controls (e.g., `textarea` or `input`)


## Configurable variables

- `--Form-input-border-color`
- `--Form-input-border-radius`
- `--Form-input-color`
- `--Form-input-font-size`
- `--Form-input-padding`
- `--Form-select-background`
- `--Form-select-background-2x`
- `--Form-select-background-width`
- `--Form-label-color`
- `--Form-label-font-size`
- `--Form-label-font-weight`
- `--Form-field-padding`
- `--Form--inline-form-field-margin`


## Usage

### Example compact form:

```html
<form class="Form">
    <fieldset>
        <label for="email">Email</label>
        <input class="Form-input" id="email" type="email" placeholder="Email">

        <label for="password">Password</label>
        <input class="Form-input" id="password" type="password" placeholder="Password">

        <input id="remember" type="checkbox">
        <label for="remember">Remember me</label>

        <button type="submit" class="Button">Sign in</button>
    </fieldset>
</form>
```

### Example of horizontally arranged label-control pairs:

```html
<form class="Form">
    <div class="Form-field">
        <label class="Form-label" for="name">Choose username</label>
        <input class="Form-input" id="name" placeholder="">
    </div>

    <div class="Form-field">
        <input id="remember" type="checkbox">
        <label for="remember">Remember me</label>
    </div>

    <button type="submit" class="Button">Sign up</button>
</form>
```

Example of a stacked form:


```html
<form class="Form">
    <div class="Form-field Form-field--stacked">
        <label class="Form-label" for="name">Choose username</label>
        <input class="Form-input" id="name" placeholder="">
    </div>

    <button type="submit" class="Button">Sign up</button>
</form>
```

See the test file for more examples.

## Testing

Install [Node](http://nodejs.org) (comes with npm).

```
npm install
```

To generate a build:

```
npm run build
```

To generate the testing build:

```
npm run build-test
```

To watch the files for making changes to test:

```
npm run watch
```

Basic visual tests are in `test/index.html`.

## Browser support

- Google Chrome (latest)
- Opera (latest)
- Firefox 4+
- Safari 5+
- Internet Explorer 8+
