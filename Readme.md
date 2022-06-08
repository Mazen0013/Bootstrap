# Bootstrap:

Bootstrap is the most popular CSS Framework for developing responsive and mobile-first websites.

Bootstrap 5 is the newest version of Bootstrap.

---

## Bootstrap Quickstrap:

there are three ways to add Bootstrap to your HTML:

1- using the bootstrap Content Delivery Network (CDN)

2- Downloading files locally
3- Using package managers to import Bootstrap to HTML

---

### 1- using the bootstrap Content Delivery Network (CDN)

Using the Bootstrap CDN is a great way to deliver the content from your website to your users quickly and efficiently based on their geographic location and improve your website server’s performance.

-To link Bootstrap in HTML using this method:
to add Bootstrap 5 CDN to HTML for CSS:

- Copy this stylesheet link to the `<head>` tag of your desired HTML file.

```
<link rel=”stylesheet” href=”https://stackpath.bootstrapcdn.com/bootstrap/5.0.0-alpha1/css/bootstrap.min.css”rel=”nofollow” integrity=”sha384-r4NyP46KrjDleawBgD5tp8Y7UzmLA05oM1iAEQ17CSuDqnUK2+k9luXQOfXJCJ4I” crossorigin=”anonymous”>
```

---

### 2- Downloading files locally:

Another way of importing Bootstrap to HTML is to directly download the files locally to your HTML project folder. The files can be downloaded from the following links:

- Bootstrap 4: https://getbootstrap.com/docs/4.3/getting-started/download/
- Bootstrap 5: https://v5.getbootstrap.com/docs/5.0/getting-started/download/

After the desired Bootstrap version files have been downloaded:

- For CSS:

Include a link to the bootstrap.min.css file in the `<head>` portion of your HTML file. Doing this enables you to use the Bootstrap CSS components as per your need.

```
<link href="css/bootstrap.min.css" rel="stylesheet">
```

---

### 3- Using package managers to import Bootstrap to HTML:

Package managers like npm and yarn can prove to be yet another efficient way of adding Bootstrap to HTML effortlessly. Since npm is the most popular package manager, the following example shows how Bootstrap can be installed and pulled into any project using it.

Type one of the following commands to the project folder. This is only valid if you have initialized npm in the project.

- Bootstrap 4: npm install bootstrap
- Bootstrap 5: npm install bootstrap@next

A local copy of the desired version of the Bootstrap files is now downloaded into the ‘node_modules’ folder in your project. After the desired Bootstrap version is imported:

- For CSS: Include the bootstap.min.css file in the <head> of your HTML file to use Bootstrap CSS components.
- For JS: Use the bootstrap.min.js file before the end of the <body> portion of your HTML file to use the Bootstrap JS components.

Once you integrate Bootstrap 4, or 5 CSS with HTML, you can simply use the Bootstrap class elements and style your HTML files in the desired manner. You can refer to the Bootstrap documentation of your desired version to understand the classes that can be used, and the actions that the corresponding classes perform. Similarly, after integrating Bootstrap JS to HTML you can use the Bootstrap JS components by using JS data attributes directly in the HTML markup or by using jQuery.

---

## Important globals:

- ### HTML5 doctype:
  Bootstrap requires the use of the HTML5 doctype. Without it, you’ll see some funky incomplete styling.

```
<!doctype html>
<html lang="en">
  ...
</html>
```

- ### Responsive meta tag:

Bootstrap is developed mobile first, a strategy in which we optimize code for mobile devices first and then scale up components as necessary using CSS media queries. To ensure proper rendering and touch zooming for all devices, add the responsive viewport meta tag to your `<head>`.

```
<meta name="viewport" content="width=device-width, initial-scale=1">
```

---

### basic HTML template using Bootstrap:

Start with this basic HTML template, you can customize it and adapt it to your needs.

```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript; choose one of the two! -->

    <!-- Option 1: Bootstrap Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>

    <!-- Option 2: Separate Popper and Bootstrap JS -->
    <!--
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js" integrity="sha384-IQsoLXl5PILFhosVNubq5LC7Qb9DXgDA9i+tQ8Zj3iwWAwPtgFTxbJ8NT4GN1R8p" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.min.js" integrity="sha384-cVKIPhGWiC2Al4u+LWgxfKTRIcfu0JTxR+EQDz/bgldoEyl4H0zUF0QKbrJ0EcQF" crossorigin="anonymous"></script>
    -->
  </body>
</html>
```

---

### Bootstrap Containers:

The container class is one of the most important Bootstrap classes and it is required when using Bootstrap's default grid system.

It provides margins, padding, alignments, and more, to HTML elements. The default .container class is a responsive, fixed-width container, meaning its max-width changes at each breakpoint.

```
<div class="container">
  <!-- content here -->

</div>
```

Bootstrap comes with three different containers:

- `.container`, which sets a max-width at each responsive breakpoint
- `.container-fluid`, which is width: 100% at all breakpoints
- `.container-{breakpoint}`, which is width: 100% until the specified breakpoint

---

### Bootstrap's Grid:

Bootstrap’s grid system uses a series of containers, rows, and columns to layout and align content. It’s built with flexbox and is fully responsive.

![grid image](/images/grid.png)

```
<div class="container">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
```

---

### Bootstrap Tables:

A boredered zebra-striped table:

![table image](/images/table.png)

```
 <table class="table table-striped table-bordered">
  <thead>
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Email</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>John</td>
      <td>Doe</td>
      <td>john@example.com</td>
    </tr>
    <tr>
      <td>Mary</td>
      <td>Moe</td>
      <td>mary@example.com</td>
    </tr>
    <tr>
      <td>July</td>
      <td>Dooley</td>
      <td>july@example.com</td>
    </tr>
  </tbody>
</table>
```

---

### Bootstrap Buttons:

Bootstrap provides different styles of buttons:

![table image](/images/buttons.png)

```
<button type="button" class="btn">Basic</button>
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-dark">Dark</button>
```

---

### Bootstrap Cards:

![table image](/images/card.png)

```
<div class="card" style="width:400px">
  <img src="img_avatar1.png" alt="Card image">
  <div class="card-body">
    <h4 class="card-title">John Doe</h4>
    <p class="card-text">Some example text.</p>
    <a href="#" class="btn btn-primary">See Profile</a>
  </div>
</div>
```

---

### Bootstrap Images:

Documentation and examples for opting images into responsive behavior (so they never become larger than their parent elements) and add lightweight styles to them—all via classes.

### Responsive images:

Images in Bootstrap are made responsive with `.img-fluid`. This applies max-width: 100%; and height: auto; to the image so that it scales with the parent element.

![table image](/images/responsive-image.png)

```
<img src="..." class="img-fluid" alt="...">
```

---

### Image thumbnails:

In addition to our border-radius utilities, you can use .img-thumbnail to give an image a rounded 1px border appearance.

![table image](/images/thumbnail-images.png)

```
<img src="..." class="img-thumbnail" alt="...">
```

### Aligning images:

Align images with the helper float classes or text alignment classes. block-level images can be centered using the .`mx-auto` margin utility class.

![table image](/images/align-images1.png)

```
<img src="..." class="rounded float-start" alt="...">
<img src="..." class="rounded float-end" alt="...">
```

![table image](/images/align-images2.png)

```
<img src="..." class="rounded mx-auto d-block" alt="...">
```

![table image](/images/align-images3.png)

```
<div class="text-center">
  <img src="..." class="rounded" alt="...">
</div>
```

---

### Bootstrap Navbar:

Documentation and examples for Bootstrap’s powerful, responsive navigation header, the navbar.

### How it works:

Here’s what you need to know before getting started with the navbar:

- Navbars require a wrapping `.navbar` with `.navbar-expand{-sm|-md|-lg|-xl|-xxl}` for responsive collapsing and color scheme classes.
- Navbars and their contents are fluid by default. Change the container to limit their horizontal width in different ways.
- Ensure accessibility by using a `<nav>` element

### Supported content:

Navbars come with built-in support for a handful of sub-components. Choose from the following as needed:

- `.navbar-brand` for your company, product, or project name.
- `.navbar-nav` for a full-height and lightweight navigation (including support for dropdowns).
- `.navbar-toggler` for use with our collapse plugin and other navigation toggling behaviors.
- `.navbar-text` for adding vertically centered strings of text.
- `.collapse.navbar-collapse` for grouping and hiding navbar contents by a parent breakpoint.

Here’s an example of all the sub-components included in a responsive light-themed navbar that automatically collapses at the lg (large) breakpoint.

![table image](/images/nav1.png)

```
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
```

This example uses background (bg-light) and spacing (my-2, my-lg-0, me-sm-0, my-sm-0) utility classes.

---

visit this [link](https://getbootstrap.com/docs/5.0/getting-started/introduction/) to read the documentation and use the proper Bootstrap classes.
