### _Bootstrap: Use Responsive Design with Bootstrap Fluid Containers_

With responsive design, there is no need to design a mobile version of your website. It will look good on devices with screens of any width.

You can add Bootstrap to any app by adding the following code to the top of your HTML:

```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous"/>
```

<!--for this page use -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous"/>

### _Bootstrap: Make Images Mobile Responsive_

- all we need to do is add the `img-responsive` class to your image. Do this, and the image should perfectly fit the width of your page.

### _Bootstrap: Center Text with Bootstrap_

- Now that we're using Bootstrap, we can center our heading element to make it look better. All we need to do is add the class `text-center` to our `h2` element.

### _Bootstrap: Create a Bootstrap Button_

- Normally, your button elements with the btn and btn-default classes are only as wide as the text that they contain. For example:

    `<button class="btn btn-default">Submit</button>`

- This button would only be as wide as the word "Submit".


- By making them block elements with the additional class of` btn-block`, your button will stretch to fill your page's entire horizontal space and any elements following it will flow onto a "new line" below the block.

    `<button class="btn btn-default btn-block">Submit</button>`

- This button would take up 100% of the available width.

### _Bootstrap: Taste the Bootstrap Button Color Rainbow_

- The `btn-primary` class is the main color you'll use in your app. It is useful for highlighting actions you want your user to take.

### _Bootstrap: Call out Optional Actions with btn-info_

- Bootstrap comes with several pre-defined colors for buttons. The `btn-info` class is used to call attention to optional actions that the user can take.

### _Bootstrap: Warn Your Users of a Dangerous Action with btn-danger_

- Bootstrap comes with several pre-defined colors for buttons. The `btn-danger` class is the button color you'll use to notify users that the button performs a destructive action, such as deleting a cat photo.

### _Bootstrap: Use the Bootstrap Grid to Put Elements Side By Side_

- Bootstrap uses a responsive 12-column grid system, which makes it easy to put elements into rows and specify each element's relative width. Most of Bootstrap's classes can be applied to a `div` element.

- Bootstrap has different column width attributes that it uses depending on how wide the user's screen is. For example, phones have narrow screens, and laptops have wider screens.

- Take for example Bootstrap's `col-md-*` class. Here, `md` means medium, and `*` is a number specifying how many columns wide the element should be. In this case, the column width of an element on a medium-sized screen, such as a laptop, is being specified.

- In the Cat Photo App that we're building, we'll use `col-xs-*`, where `xs` means extra small (like an extra-small mobile phone screen), and `*` is the number of columns specifying how many columns wide the element should be.

### _Bootstrap: Use a span to Target Inline Elements_

- By using the inline `span` element, you can put several elements on the same line, and even style different parts of the same line differently.

```html
<p>Top 3 things cats <span class="text-danger">hate:</span></p>
```

### _Bootstrap: Add Font Awesome Icons to our Buttons_

- Font Awesome is a convenient library of icons. These icons can be webfonts or vector graphics. These icons are treated just like fonts. You can specify their size using pixels, and they will assume the font size of their parent HTML elements.

- You can include Font Awesome in any app by adding the following code to the top of your HTML:

<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">

- In this case, we've already added it for you to this page behind the scenes.

- The `i` element was originally used to make other elements italic, but is now commonly used for icons. You can add the Font Awesome classes to the `i` element to turn it into an icon, for example:

- Note that the span element is also acceptable for use with icons.

```html
<i class="fas fa-info-circle"></i>
```

- Use Font Awesome to add a `thumbs-up` icon to your like button by giving it an `i` element with the classes `fas` and `fa-thumbs-up`. Make sure to keep the text "Like" next to the icon.

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
```

<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>

### _Bootstrap: Add Font Awesome Icons to all of our Buttons_

- Font Awesome is a convenient library of icons. These icons can be web fonts or vector graphics. These icons are treated just like fonts. You can specify their size using pixels, and they will assume the font size of their parent HTML elements.

- Use Font Awesome to amdd an `info-circle` icon to your info button and a `trash` icon to your delete button.

- Note: The `span` element is an acceptable alternative to the `i` element for the directions below.

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
```

<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>

### _Bootstrap: Responsively Style Radio Buttons_

- You can use Bootstrap's `col-xs-*` classes on `form` elements, too! This way, our radio buttons will be evenly spread out across the page, regardless of how wide the screen resolution is.

### _Bootstrap: Responsively Style Checkboxes_

- Since Bootstrap's `col-xs-*` classes are applicable to all `form` elements, you can use them on your checkboxes too! This way, the checkboxes will be evenly spread out across the page, regardless of how wide the screen resolution is.

### _Bootstrap: Style Text Inputs as Form Controls_

- You can add the `fa-paper-plane` Font Awesome icon by adding `<i class="fa fa-paper-plane"></i>` within your submit `button` element.

- Give your form's text input field a class of `form-control`. Give your form's submit button the classes `btn btn-primary`. Also give this button the Font Awesome icon of `fa-paper-plane`.

- All textual `<input>`, `<textarea>`, and `<select>` elements with the class `.form-control` have a width of 100%.

  ```html
   <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <input class="form-control" type="text" placeholder="cat photo URL" required>
    <button class="btn btn-primary" type="submit"><i class="fa fa-paper-plane">Submit</i></button>
  </form>
```

  <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <input class="form-control" type="text" placeholder="cat photo URL" required>
    <button class="btn btn-primary" type="submit"><i class="fa fa-paper-plane">Submit</i></button>
  </form>

### _Bootstrap: Line up Form Elements Responsively with Bootstrap_

- Now let's get your form `input` and your submission `button` on the same line. We'll do this the same way we have previously: by using a `div` element with the class `row`, and other `div` elements within it using the `col-xs-*` class.

- Nest both your form's text i`nput` and submit `button` within a `div` with the class `row`. Nest your form's text `input` within a `div` with the class of `col-xs-7`. Nest your form's submit `button` in a `div` with the class `col-xs-5`.

```html
   <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-7">
        <input  type="text" class="form-control" placeholder="cat photo URL" required>
      </div>
      <div class="col-xs-5">
        <button class="col-xs-5" type="submit" class="btn btn-primary"><i class="fa fa-paper-plane"></i> Submit</button>
      </div>
    </div>
  </form>
```

  <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-7">
        <input  type="text" class="form-control" placeholder="cat photo URL" required>
      </div>
      <div class="col-xs-5">
        <button class="col-xs-5" type="submit" class="btn btn-primary"><i class="fa fa-paper-plane"></i> Submit</button>
      </div>
    </div>
  </form>

#### This is the last challenge we'll do for our Cat Photo App for now

<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-7">
        <input type="text" class="form-control" placeholder="cat photo URL" required>
      </div>
      <div class="col-xs-5">
        <button type="submit" class="btn btn-primary"><i class="fa fa-paper-plane"></i> Submit</button>
      </div>
    </div>
  </form>
</div>

### _Bootstrap: Create a Bootstrap Headline_

- To start with, create an `h3` element, with the text `jQuery Playground`.

- Color your `h3` element with the `text-primary` Bootstrap class, and center it with the `text-center` Bootstrap class.

```html
<h3 class="text-primary text-center">jQuery Playground</h3>
```

<h3 class="text-primary text-center">jQuery Playground</h3>

### _Bootstrap: House our page within a Bootstrap container-fluid div_

- Now let's make sure all the content on your page is mobile-responsive.

- Let's nest your `h3` element within a `div` element with the class `container-fluid`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
</div>

### _Bootstrap: Create a Bootstrap Row_

- Now we'll create a Bootstrap row for our inline elements.

- Create a `div` element below the `h3` tag, with a class of `row`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
  </div>
</div>
```

### _Bootstrap: Split Your Bootstrap Row_

- Now that we have a Bootstrap Row, let's split it into two columns to house our elements.

- Create two `div` elements within your row, both with the class `col-xs-6`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
    </div>
    <div class="col-xs-6">
    </div>
  </div>
</div>
```

### _Bootstrap: Create Bootstrap Wells_

- Bootstrap has a class called `well` that can create a visual sense of depth for your columns.

- Nest one `div` element with the class `well` within each of your `col-xs-6` `div` elements.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Add Elements within Your Bootstrap Wells_

- Nest three `button` elements within each of your `well` `div` elements.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
  </div>
</div>


### _Bootstrap: Apply the Default Bootstrap Button Style_

- Bootstrap has another button class called `btn-default`.

- Apply both the `btn` and `btn-default` classes to each of your `button` elements.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Create a Class to Target with jQuery Selectors_

- Not every class needs to have corresponding CSS. Sometimes we create classes just for the purpose of selecting these elements more easily using jQuery.

- Give each of your `button` elements the class `target`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Add id Attributes to Bootstrap Elements_

- Recall that in addition to class attributes, you can give each of your elements an `id` attribute.

- Each id must be unique to a specific element and used only once per page.

- Let's give a unique id to each of our `div` elements of class `well`.

- Remember that you can give an element an id like this:

    `<div class="well" id="center-well">`

- Give the well on the left the id of `left-well`. Give the well on the right the id of `right-well`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Label Bootstrap Wells_

- For the sake of clarity, let's label both of our wells with their ids.

- Above your left-well, inside its `col-xs-6` `div` element, add a `h4` element with the text `#left-well`.

- Above your right-well, inside its `col-xs-6` `div` element, add a `h4` element with the text `#right-well`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Give Each Element a Unique id_

- We will also want to be able to use jQuery to target each button by its unique id.

- Give each of your buttons a unique id, starting with `target1` and ending with `target6`.

- Make sure that `target1` to `target3` are in `#left-well`, and `target4` to `target6` are in `#right-well`.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1"></button>
        <button class="btn btn-default target" id="target2"></button>
        <button class="btn btn-default target" id="target3"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4"></button>
        <button class="btn btn-default target" id="target5"></button>
        <button class="btn btn-default target" id="target6"></button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1"></button>
        <button class="btn btn-default target" id="target2"></button>
        <button class="btn btn-default target" id="target3"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4"></button>
        <button class="btn btn-default target" id="target5"></button>
        <button class="btn btn-default target" id="target6"></button>
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Label Bootstrap Buttons_

- Give each of your button elements text that corresponds to its id's selector.

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

### _Bootstrap: Use Comments to Clarify Code_

- When we start using jQuery, we will modify HTML elements without needing to actually change them in HTML.

- Let's make sure that everyone knows they shouldn't actually modify any of this code directly.

- Remember that you can start a comment with `<!--` and end a comment with `-->`

- Add a comment at the top of your HTML that says `Only change code above this line`.

```html
<!-- Only change code abobe this line-->
```
