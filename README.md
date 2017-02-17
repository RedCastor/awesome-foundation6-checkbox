Awesome Foundation6 Checkbox
==========================

[Font Awesome][] [Foundation 6][] Checkboxes & Radios plugin. Pure CSS way to make inputs look prettier. **No Javascript!**

**[Demo][]**

Use
------------

First just include **awesome-foundation-checkbox.css** somewhere in your HTML, or add the equivalent files to your [Sass](#using-sass) configuration.

````html
<form role="form">
  ...
  <div class="checkbox">
    <label>
      <input type="checkbox"> Check me out
    </label>
  </div>
  ...
</form>
````

We have to alter it a bit:
````html
<form role="form">
  ...
  <div class="checkbox">
    <input type="checkbox" id="checkbox1">
    <label for="checkbox1">
        Check me out
    </label>
  </div>
  ...
</form>
````
That's it. It will work. But it **will not** work if you nest input inside label or put label before input.

If you want to enable **Opera 12** and earlier support  just add class `styled` to `input` element:
````html
...
<input type="checkbox" id="checkbox1" class="styled">
...
````

Browser support
-----------
- Firefox (_3.6+_)
- Chrome  (_14+_)
- IE      (_9+_)
- Opera   (_11.6+_)
- Safari  (_6+_)

Radios
------------

It's the same for radios. Markup has to be the following:
````html
<form role="form">
  ...
  <div class="radio">
      <input type="radio" name="radio2" id="radio3" value="option1">
      <label for="radio3">
          One
      </label>
  </div>
  <div class="radio">
      <input type="radio" name="radio2" id="radio4" value="option2" checked>
      <label for="radio4">
          Two
      </label>
  </div>
  ...
</form>
````

Brand Colors and other features
------------

You may use `primary`, `alert`, `secondary`, etc to style checkboxes and radios with base foundation colors.

`checkbox-circle` is for rounded checkboxes.

Inputs without label text:

````html
<div class="checkbox">
  <input type="checkbox" class="styled" id="singleCheckbox1" value="option1" aria-label="Single checkbox One">
  <label></label>
</div>
````

Using [Sass][]
----------

As per example in the `demo` folder, to use Font Awesome you'll have to `@import` the following library parts:

````scss
@import "../bower_components/foundation-sites/assets/foundation";
@import "../bower_components/font-awesome/scss/variables";

@import "../awesome-foundation6-checkbox";
````

Adjust this to the path where your foundation and font-awesome files are located.


Credits
------------

Based on the [Official Foundation6 Sass port][Foundation6 Sass] and the awesome [Font Awesome][].


[Demo]: http://redcastor.github.io/awesome-foundation6-checkbox/demo/
[Foundation 6]: https://foundation.zurb.com/sites/docs/
[v1.0.0]: https://github.com/redcastor/awesome-foundation6-checkbox/releases/tag/v1.0.0
[Foundation 6 Sass]: https://github.com/zurb/foundation-sites
[Font Awesome]: https://github.com/FortAwesome/Font-Awesome
[Sass]: http://sass-lang.com/
