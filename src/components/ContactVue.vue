<template>
  <section id="contact">
    <div class="container-fluid overlay h-100 d-flex align-items-center">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <h3>Need help? Just contact us.</h3>
            <div class="kontak">
              <h6>Contact</h6>
              <div class="mbb">
                <img src="/assets/img/icons8-place-marker-96.png" alt="">
                <a href="#">Jl. Kenanga No.123 Kediri, Jawa Timur</a>
              </div>
              <div class="mbb">
                <img src="/assets/img/icons8-phone-96.png" alt="">
                <a href="#">0354-0123456</a>
              </div>
              <div class="mbb">
                <img src="/assets/img/icons8-mail-96.png" alt="">
                <a href="#">mail.dekoruma@email.com</a>
              </div>
              
              <div class="sosmed mt-5">
                <h6>Follow us on social media</h6>
                <a href="#"><img src="/assets/img/icons8-facebook-96.png" alt=""></a>
                <a href="#"><img src="/assets/img/icons8-instagram-96.png" alt=""></a>
                <a href="#"><img src="/assets/img/icons8-twitter-96.png" alt=""></a>
              </div>
            </div>
          </div>

          <div class="col-md-6">
            <div class="card-contact w-100">
              <form action="">
                <div class="form-floating mb-3">
                  <input type="text" class="form-control" id="floatingInput" placeholder="name@example.com">
                  <label for="floatingInput">Name</label>
                </div>
                <div class="form-floating mb-3">
                  <input type="email" class="form-control" id="floatingInput" placeholder="name@example.com">
                  <label for="floatingInput">Email address</label>
                </div>
                <div class="form-floating">
                  <textarea class="form-control" placeholder="Leave a comment here" id="floatingTextarea2" style="height: 100px"></textarea>
                  <label for="floatingTextarea2">Comments</label>
                </div>
                <button type="submit" class="btn-submit rounded-pill mt-3">Send</button>
              </form>
            </div>  
          </div>
        </div>
      </div>
    </div>

  </section>
</template>