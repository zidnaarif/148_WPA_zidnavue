<template>
<nav class="navbar navbar-expand-lg navbar-light bg-transparent position-fixed w-100">
    <div class="container">
      <a class="navbar-brand" href="/">
        <img src="/assets/img/logo.png" alt="" width="30" class="d-inline-block align-text-top">
        Dekoruma
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mx-auto">
          <li class="nav-item mx-2">
            <a class="nav-link active" aria-current="page" href="/">Home</a>
          </li>
          <li class="nav-item mx-2">
            <a class="nav-link" href="/pricing.html">Pricing</a>
          </li>
          <li class="nav-item mx-2">
            <a class="nav-link" href="/contact.html">Contact</a>
          </li>
          <li class="nav-item mx-2">
            <a class="nav-link" href="/about.html">About</a>
          </li>
        </ul>

        <div>
          <button class="button-primary" onclick="location.href='/register.html'">Register</button>
          <button type="button" class="button-secondary rounded-pill" data-bs-toggle="modal" data-bs-target="#LoginModal">Login</button>
        </div>

      </div>
    </div>
  </nav>

      <!-- Modal -->
    <div class="modal fade" id="LoginModal" tabindex="-1" aria-labelledby="LoginModalLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="LoginModalLabel">Login</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            <div class="mb-3 ms-2 me-2">
              <label for="emailinput" class="form-label">Email address</label>
              <input type="email" class="form-control rounded-pill" id="emailinput" placeholder="name@example.com">
            </div>
            <div class="mb-3 ms-2 me-2">
              <label for="inputPassword" class="col-sm-2 col-form-label">Password</label>
              <input type="password" class="form-control rounded-pill" id="inputPassword">
            </div>
          </div>
          <div class="modal-footer me-2">
            <a class="nav-link fst-italic" href="#">Forgot Password</a>
            <button type="button" class="button-secondary rounded-pill">Login</button>
          </div>
        </div>
      </div>
    </div>
    <!-- End of Modal -->

</template>
