# bulma-divider
Bulma's extension to easily display an horizontal or vertical divider
(find all my bulma's extensions [here](https://github.com/Wikiki/bulma-extensions))

Usage
-----

```html
<div class="divider"></div>
<div class="divider" data-content="OR"></div>
<div class="columns">
  <div class="column">
    <form>
      <div class="form-group">
        <label class="form-label" for="input-example-1">Email</label>
        <input class="form-input" id="input-example-1" placeholder="Email" type="text">
      </div>
      <div class="form-group">
        <label class="form-label" for="input-example-2">Password</label>
        <input class="form-input" id="input-example-2" placeholder="Password" autocomplete="new-password" type="password">
      </div>
      <div class="form-group">
        <label class="form-checkbox">
        <input type="checkbox">
        <i class="form-icon"></i> Remember me
      </label>
      </div>
      <div class="form-group">
        <button class="btn btn-primary">Sign in</button>
      </div>
    </form>
  </div>
  <div class="divider-vert" data-content="OR"></div>
  <div class="column">
    <form>
      <div class="form-group">
        <label class="form-label" for="input-example-1">Email</label>
        <input class="form-input" id="input-example-1" placeholder="Email" type="text">
      </div>
      <div class="form-group">
        <label class="form-label" for="input-example-2">Password</label>
        <input class="form-input" id="input-example-2" placeholder="Password" autocomplete="new-password" type="password">
      </div>
      <div class="form-group">
        <label class="form-checkbox">
        <input type="checkbox">
        <i class="form-icon"></i> Remember me
      </label>
      </div>
      <div class="form-group">
        <button class="btn btn-primary">Sign in</button>
      </div>
    </form>
  </div>
</div>
```

Variables
---
This extension uses Bulma's color modifiers and have the following variables

Name | Description | Default value    
-----|-------------|---------------
$divider-background-color | Divider line color | $grey-lighter
$divider-font-size | Font size of divider text | $size-7
$divider-color | Color or divider text | $grey-light

Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `divider.sass`
- Copy the code form the `bulma-divider repo`'s [divider.sass](https://github.com/Wikiki/bulma-divider/blob/master/divider.sass) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"
@import "divider.sass"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
