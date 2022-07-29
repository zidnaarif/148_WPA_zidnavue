<template>

    <NavbarVue/>

    <section id="register">
    <div class="container-fluid overlay">
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <div class="title position-relative top-50 start-50 translate-middle mb-5">
                        <h3>Create a Dekoruma ID</h3>
                        <span>One last step before starting your free 14-day trial.</span>
                    </div>
                </div>

                <div class="col-md-6">
                    <div class="FormRegister">
                        <form action="">
                            <div class="mb-3 ms-2 me-2">
                                <label for="nameinput" class="form-label">Name</label>
                                <input type="text" class="form-control rounded-pill" id="nameinput">
                            </div>
                            <div class="mb-3 ms-2 me-2">
                                <label for="emailinput" class="form-label">Email address</label>
                                <input type="email" class="form-control rounded-pill" id="emailinput" placeholder="name@example.com">
                            </div>
                            <div class="mb-3 ms-2 me-2">
                                <label for="inputPassword" class="col-sm-2 col-form-label">Password</label>
                                <input type="password" class="form-control rounded-pill" id="inputPassword">
                            </div>
                            <div class="mb-3 ms-2 me-2">
                                <label for="inputPassword" class="col-sm-4 col-form-label">Repeat Password</label>
                                <input type="password" class="form-control rounded-pill" id="inputPassword">
                            </div>
                            <button type="submit" class="position-relative btn-submit rounded-pill mt-3 mb-3 start-50 translate-middle-x">Submit</button>
                            <div class="note ms-2 mt-3">
                                <span>By proceeding, you agree to the <a href="#">Terms and Conditions</a></span>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
    </section>

    <FooterVue/>

</template>

<script>
import NavbarVue from '@/components/NavbarVue.vue'
import FooterVue from '@/components/FooterVue.vue'

export default {
    setup() {
    },
    mounted() {
        document.title = "Register";
    },
    components: { 
        NavbarVue,
        FooterVue
    }
}
</script>
