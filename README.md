# -BootStrap
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap 5 Feature Showcase</title>
  <link rel="stylesheet" href="bootstrap/css/bootstrap.min.css">
  <link rel="stylesheet" href="css/custom.css">
  <link rel="stylesheet" href="icons/bootstrap-icons.css">
</head>
<body>
  <!-- Navbar (Exercise 10.1, 7.1) -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Showcase</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item"><a class="nav-link active" href="#grid-layouts">Grid</a></li>
          <li class="nav-item"><a class="nav-link" href="#forms-buttons">Forms</a></li>
          <li class="nav-item"><a class="nav-link" href="#cards-media">Cards</a></li>
          <li class="nav-item"><a class="nav-link" href="#interactive">JS Plugins</a></li>
        </ul>
        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search">
          <button class="btn btn-outline-light" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>

  <!-- Grid & Layout (Exercises 3, 4, 5) -->
  <section id="grid-layouts" class="container mt-5">
    <h2 class="mb-4">Responsive Grid Layouts</h2>
    <div class="row">
      <div class="col-12 col-md-6 col-lg-4 bg-light p-3">Column 1</div>
      <div class="col-12 col-md-6 col-lg-4 bg-secondary text-white p-3">Column 2</div>
      <div class="col-12 col-md-12 col-lg-4 bg-light p-3">Column 3</div>
    </div>
    <div class="row mt-4 align-items-center justify-content-center">
      <div class="col-md-3 order-md-2 bg-warning p-3">Reordered Second</div>
      <div class="col-md-3 order-md-1 bg-info p-3">Reordered First</div>
    </div>
  </section>

  <!-- Typography & Spacing Utilities (7, 12) -->
  <section id="typography" class="container mt-5">
    <h2 class="display-4 text-center">Typography Showcase</h2>
    <p class="lead text-muted">This is a lead paragraph. <span class="fw-bold text-uppercase">Bold uppercase</span> and <span class="text-lowercase">lowercase</span>.</p>
    <div class="mt-4 p-3 bg-light m-3 rounded">Box with spacing (m-3, p-3)</div>
  </section>

  <!-- Forms & Buttons (8, 9) -->
  <section id="forms-buttons" class="container mt-5">
    <h2>Forms and Buttons</h2>
    <form class="mb-4">
      <div class="mb-3">
        <label class="form-label">Username</label>
        <input type="text" class="form-control">
      </div>
      <div class="mb-3 form-check">
        <input type="checkbox" class="form-check-input" id="check1">
        <label class="form-check-label" for="check1">Accept Terms</label>
      </div>
      <div class="input-group mb-3">
        <span class="input-group-text">@</span>
        <input type="text" class="form-control" placeholder="Twitter Handle">
      </div>
      <div class="form-floating mb-3">
        <input type="email" class="form-control" id="floatingEmail" placeholder="name@example.com">
        <label for="floatingEmail">Email address</label>
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
      <button type="button" class="btn btn-outline-secondary">Cancel</button>
    </form>
    <div class="btn-group" role="group">
      <input type="checkbox" class="btn-check" id="btn-check1" autocomplete="off">
      <label class="btn btn-outline-success" for="btn-check1">Toggle</label>
    </div>
  </section>

  <!-- Cards & Media (11) -->
  <section id="cards-media" class="container mt-5">
    <h2>Cards and Media</h2>
    <div class="card mb-3" style="width: 18rem;">
      <img src="img/profile.jpg" class="card-img-top rounded-circle" alt="Profile">
      <div class="card-body">
        <h5 class="card-title">Ram</h5>
        <p class="card-text">Web Developer</p>
      </div>
    </div>
    <div class="d-flex align-items-start">
      <img src="img/profile.jpg" alt="media" width="64" height="64" class="me-3 rounded">
      <div>
        <h5>Media Title</h5>
        <p>This is a media object example with text beside an image.</p>
      </div>
    </div>
  </section>

  <!-- Styling (13, 14, 15) -->
  <section id="styling" class="container mt-5">
    <div class="row">
      <div class="col-md-4 bg-primary text-white p-4">Primary BG</div>
      <div class="col-md-4 bg-warning text-dark p-4">Warning BG</div>
      <div class="col-md-4 bg-dark text-white bg-gradient p-4">Dark Gradient</div>
    </div>
    <div class="mt-4 d-none d-md-block">This is hidden on small screens.</div>
    <img src="img/profile.jpg" class="border border-3 border-primary rounded-circle mt-4" width="100">
    <div class="card shadow-lg rounded-pill mt-4 p-3">Pill card with shadow</div>
  </section>

  <!-- Positioning (16) -->
  <section id="positioning" class="container mt-5 position-relative">
    <img src="img/profile.jpg" class="img-fluid" alt="Main Image">
    <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">New</span>
  </section>

  <!-- JS Plugins & Icons (17, 18) -->
  <section id="interactive" class="container mt-5">
    <h2>JS Plugins and Icons</h2>
    <button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">Launch Modal</button>
    <div class="modal fade" id="exampleModal" tabindex="-1">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title">Modal title</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
          </div>
          <div class="modal-body">Hello</div>
          <div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
          </div>
        </div>
      </div>
    </div>
    <div class="accordion mt-4" id="accordionExample">
      <div class="accordion-item">
        <h2 class="accordion-header">
          <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne">
            Accordion Item #1
          </button>
        </h2>
        <div id="collapseOne" class="accordion-collapse collapse show">
          <div class="accordion-body">This is the first item's accordion body.</div>
        </div>
      </div>
    </div>
    <div class="mt-4">
      <a href="#" class="text-decoration-none"><i class="bi bi-facebook"></i></a>
      <a href="#" class="text-decoration-none"><i class="bi bi-twitter"></i></a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-dark text-white text-center py-3 position-fixed bottom-0 w-100">
  End
  </footer>

  <script src="bootstrap/js/bootstrap.bundle.min.js"></script>
  <script src="js/main.js"></script>
</body>
</html>
