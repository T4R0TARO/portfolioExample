# NAVBAR SECTION 
```scss
@use '../custom' as *;
@use '../components/mixins' as *;

// Style the background color and font
.menu {
    @include gradient;

    li {
        padding: 0 0.7rem;

        a {
            color: $white !important;
            text-transform: capitalize;
            font-weight: 600;
        }
    }
}

``` 
```html
<nav class="navbar navbar-expand-lg navbar-dark menu shadow fixed-top">
    <div class="container">
      <!-- LOGO IMAGE -->
      <a class="navbar-brand" href="#">
        <img src="images/logo1.png" alt="logo images" id="logo">
      </a>
      <!-- MOBILE BUTTON START -->
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <!-- NAV ITEMS COLLAPSE START -->
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Services</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Testimonials</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">faq</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">portfolio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">contacts</a>
          </li>
        </ul>
        <!-- PHONE BUTTON -->
        <button type="button" class="rounded-pill btn-rounded">+1 999-999-9999
            <span>
              <i class="fas fa-phone-alt"></i>
            </span>
        </button>
      </div>
    </div>
  </nav>
```

