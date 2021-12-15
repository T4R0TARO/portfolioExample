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

# INTRO SECTION 
- glightbox (video)
- button animation

```html
<section id="home" class="intro-section">
  <div class="container">
    <div class="row align-items-center text-white">
      <!-- START THE CONTENT FOR THE INTRO -->
      <div class="col-md-6 intros">
        <h1 class="display-2">
          <span class="display-2--intro">Hey!, I'm Josh</span>
          <span class="display-2--description lh-base">this is a multi-purpose responsive layout created with bootstrap v5.(here your can place your description text)   
          </span>
        </h1>
        <button type="button" class="rounded-pill btn-rounded">Get in Touch
          <span>
            <i class="fas fa-arrow-right"></i>
          </span>
        </button>
      </div>

      <!-- START THE CONTENT FOR THE VIDEO -->
      <div class="col-md-6 intros text-end">
        <div class="video-box">
          <img src="images/art/intro-section-illustration.png" alt="video illustration" class="img-fluid">
          <a href="#" class="glightbox position-absolute top-50 start-50 translate-middle">
            <span>
              <i class="fas fa-play-circle"></i>
            </span>
            <span class="border-animation border-animation--border-1"></span>
            <span class="border-animation border-animation--border-2"></span>
          </a>
        </div>
      </div>
    </div>
  </div>
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#fff" fill-opacity="1" d="M0,128L40,154.7C80,181,160,235,240,218.7C320,203,400,117,480,117.3C560,117,640,203,720,234.7C800,267,880,245,960,202.7C1040,160,1120,96,1200,85.3C1280,75,1360,117,1400,138.7L1440,160L1440,320L1400,320C1360,320,1280,320,1200,320C1120,320,1040,320,960,320C880,320,800,320,720,320C640,320,560,320,480,320C400,320,320,320,240,320C160,320,80,320,40,320L0,320Z" style="--darkreader-inline-fill: #007acc;" data-darkreader-inline-fill=""></path></svg>
</section>

```