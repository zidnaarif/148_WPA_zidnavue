<template>
    <footer class="d-flex align-items-center position-relative">
        <div class="container-fluid">
        <div class="container">
            <div class="row">
            <div class="col-md-7 d-flex align-items-center">
                <img src="/assets/img/realestate-logo.png" alt="">
                <a href="#" class="ms-2"><h5>Dekoruma</h5></a>
            </div>
            <div class="link col-md-5 d-flex justify-content-evenly">
                <router-link to="/">Home</router-link>
                <router-link to="/pricing">Pricing</router-link>
                <router-link to="/contact">Contact</router-link>
                <router-link to="/about">About</router-link>
            </div>
            </div>
            <div class="row position-absolute copyright start-50 translate-middle">
            <p>Copyright &copy;Dekoruma All Right Reserved.</p>
            </div>
        </div>
        </div>
    </footer>
</template>