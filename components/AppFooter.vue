<template>
    <!-- Footer -->
    <div class="container text-center text-md-start footer-block">
        <!-- Grid row -->
        <div class="row mx-5 mt-5">
            <!-- Grid column -->
            <div class="col-md-6 col-lg-6 col-xl-6 mx-auto mb-4">
                <!-- Content -->
                <img class="footer-logo" :src="require(`~/assets/logo.svg`)" />
                <p class="footer-copy-right">&copy; Driveclub. All rights reserved.</p>
            </div>
            <!-- Grid column -->
            <!-- Grid column -->
            <div class="col-md-3 col-lg-3 col-xl-3 mx-auto mb-4">
                <!-- Links -->
                <h6 class="text-uppercase fw-bold footer-list-header">Models</h6>
                <p>
                    <a href="#!" class="text-white">LA FERRARI</a>
                </p>
                <p>
                    <a href="#!" class="text-white">MODEL S</a>
                </p>
            </div>
            <!-- Grid column -->
            <!-- Grid column -->
            <div class="col-md-3 col-lg-3 col-xl-3 mx-auto mb-md-0 mb-4">
                <!-- Links -->
                <h6 class="text-uppercase fw-bold footer-list-header">More</h6>
                <p>
                    <a href="#!" class="text-white">HOME</a>
                </p>
                <p>
                    <a href="#!" class="text-white">CONTACT US</a>
                </p>
            </div>
            <!-- Grid column -->
        </div>
        <!-- Grid row -->
    </div>
</template>

<script>
    export default {
        name: "AppFooter"
    };
</script>

<style>
    @media only screen and (min-width: 768px) {
        .footer-list-header {
            color: #ffffff !important;
        }

        .footer-copy-right {
            text-align: left;
            font: normal normal 300 14px/21px Poppins;
            letter-spacing: 0.56px;
            color: #FFFFFF;
            opacity: 0.48;
        }
    }


    @media only screen and (max-width: 767px) {
        .footer-list-header {
            color: #ffffff !important;
        }

        .footer-copy-right {
            text-align: center;
            font: normal normal 300 14px/21px Poppins;
            letter-spacing: 0.56px;
            color: #FFFFFF;
            opacity: 0.48;
        }
    }

    .footer-block {
        background-color: #22282D;
        border-top: 1px solid #ffffff;
    }
</style>
