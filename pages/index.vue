<template>
    <div>
        <div class="hero-image border-bottom">
            <div class="hero-text">
                <h1>{{ heroTitle }}</h1>
                <h3>COME STANDARD</h3>
                <p>Discover the benefits of DRIVECLUB Trade-in and get a free vehicle evaluation.</p>
            </div>
        </div>
        <div class="page-content desktop-view">
            <!-- new div -->
            <div class="split-wrap">
                <div class="split first">
                    <div class="cover">
                        <div class="text-box">
                            <h6 class="new-range">NEW RANGE</h6>
                            <h1 class="car-model">LA FERRARI</h1>
                            <h6 class="learn-more"  onclick="document.getElementById('ferrari-modal').style.width = '100%';">LEARN MORE</h6>
                        </div>
                    </div>
                </div>
                <div class="split second border-left">
                    <div class="cover">
                        <img src="/assets/car-1.jpg">
                    </div>
                </div>
            </div>
            <!-- new div -->
            <div class="split-wrap">
                <div class="split second border-right border-top">
                    <div class="cover">
                        <img src="/assets/car-2.jpg">
                    </div>
                </div>
                <div class="split first">
                    <div class="cover">
                        <div class="text-box">
                            <h6 class="new-range">NEW RANGE</h6>
                            <h1 class="car-model">MODEL S</h1>
                            <h6 class="learn-more"  onclick="document.getElementById('ferrari-modal').style.width = '100%';">LEARN MORE</h6>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="page-content mobile-view">
            <!-- new div -->
            <div class="split-wrap">
                <div class="split second border-bottom">
                    <div class="cover">
                        <img src="/assets/car-1.jpg">
                    </div>
                </div>
                <div class="split first">
                    <div class="cover">
                        <div class="text-box">
                            <h6 class="new-range">NEW RANGE</h6>
                            <h1 class="car-model">LA FERRARI</h1>
                            <h6 class="learn-more"  onclick="document.getElementById('ferrari-modal').style.width = '100%';">LEARN MORE</h6>
                        </div>
                    </div>
                </div>
            </div>
            <!-- new div -->
            <div class="split-wrap">
                <div class="split second border-top border-bottom">
                    <div class="cover">
                        <img src="/assets/car-2.jpg">
                    </div>
                </div>
                <div class="split first">
                    <div class="cover">
                        <div class="text-box">
                            <h6 class="new-range">NEW RANGE</h6>
                            <h1 class="car-model">MODEL S</h1>
                            <h6 class="learn-more"  onclick="document.getElementById('ferrari-modal').style.width = '100%';">LEARN MORE</h6>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- The overlays -->
        <div id="ferrari-modal" class="overlay">
            <!-- Button to close the overlay navigation -->
            <a href="javascript:void(0)" class="closebtn" onclick="document.getElementById('ferrari-modal').style.width = '0%';">&times;</a>
            <!-- Overlay content -->
            <div class="overlay-content">
                <div class="split-wrap">
                    <div class="split second">
                        <div class="cover">
                            <img src="/assets/car-large.jpg">
                        </div>
                    </div>
                    <div class="split first">
                        <div class="cover">
                            <div class="text-box">
                                <h6 class="new-range">NEW RANGE</h6>
                                <h1 class="car-model">LA FERRARI</h1>
                                <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. <br><br>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. <br><br>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. <br><br>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. <br><br>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit</p>
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        head() {
            return {
                title: "Home",
                meta: [
                    {
                      hid: "description",
                      name: "description",
                      content: "Home page"
                    }
                ]
            };
        },
        data() {
            return {
                heroTitle: "GOOSEBUMPS"
            }
        }
    };


</script>
<style>

.border-left {
    border-left: 1px solid #ffffff;
}

.border-top {
    border-top: 1px solid #ffffff;
}

.border-right {
    border-right: 1px solid #ffffff;
}

.border-bottom {
    border-bottom: 1px solid #ffffff;
}

.overlay-content .text-box {
    width:80%;
    display: block;
    overflow-x: scroll;
    height: 100vh;
}

.overlay-content p {
    text-align: left;
}

.overlay-content .split.first {
    margin-top: 100px;
}
    /** overlay **/

    /* The Overlay (background) */
    .overlay {
        /* Height & width depends on how you want to reveal the overlay (see JS below) */
        height: 100%;
        width: 0;
        position: fixed;
        /* Stay in place */
        z-index: 1;
        /* Sit on top */
        left: 0;
        top: 0;
        background-color: rgb(0, 0, 0);
        /* Black w/opacity */
        overflow-x: hidden;
        /* Disable horizontal scroll */
        transition: 0.5s;
        /* 0.5 second transition effect to slide in or slide down the overlay (height or width, depending on reveal) */
        z-index: 9999;
    }

    /* Position the content inside the overlay */
    .overlay-content {
        position: relative;
        /* 25% from the top */
        width: 100%;
        /* 100% width */
        text-align: center;
        /* Centered text/links */
        /* 30px top margin to avoid conflict with the close button on smaller screens */
    }

    /* The navigation links inside the overlay */
    .overlay a {
        padding: 8px;
        text-decoration: none;
        font-size: 36px;
        color: #818181;
        display: block;
        /* Display block instead of inline */
        transition: 0.3s;
        /* Transition effects on hover (color) */
    }

    /* When you mouse over the navigation links, change their color */
    .overlay a:hover,
    .overlay a:focus {
        color: #f1f1f1;
    }

    /* Position the close button (top right corner) */
    .overlay .closebtn {
        position: absolute;
        top: 0px;
        right: 30px;
        font-size: 60px;
    }

    /* When the height of the screen is less than 450 pixels, change the font-size of the links and position the close button again, so they don't overlap */
    @media screen and (max-height: 450px) {
        .overlay a {
            font-size: 20px
        }

        .overlay .closebtn {
            font-size: 40px;
            top: 15px;
            right: 35px;
        }
    }


    /** overlay **/







    @media only screen and (min-width: 768px) {

        .nav-home {
            text-align: center;
            letter-spacing: 0.64px;
            color: #FF0050 !important;
            opacity: 1;
            border-top: 3px solid #FF0050;
        }

        .mobile-view {
            display: none;
        }

        .hero-image {
            background-image: url("/assets/hero-home.jpg");
            background-color: #cccccc;
            height: 600px;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            position: relative;
            margin-top: -84px;

        }

        .hero-text {
            position: absolute;
            top: 200px;
            left: 100px;
            color: white;
        }

        .hero-text h1 {
            font-size:50px
        }

        .text-box {
            margin: auto;
            width: 300px;
        }

        .split-wrap {
            background-color: #171B1E;
        }

        .split.first {
            margin-top: 15%;
            width: 40%;
            display: block;
            float: left;
            overflow: hidden;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;

        }

        .split.second {
            width: 60%;
            display: block;
            float: left;
            overflow: hidden;

            -webkit-transition: -webkit-transform 1s ease;
            transition: -webkit-transform 1s ease;
            transition: transform 1s ease;
            transition: transform 1s ease, -webkit-transform 1s ease;
            max-width: 100%;
            max-height: 100%;
        }


        .page-content .split.second:hover {
            -webkit-transform: scale(1.2);
            transform: scale(1.2);

        }

        .split.second img {
            width: 100%;
            height: auto;
            -webkit-transition: -webkit-transform 1s ease;
            transition: -webkit-transform 1s ease;
            transition: transform 1s ease;
            transition: transform 1s ease, -webkit-transform 1s ease;
        }

        .page-content .split.second:hover img {
            -webkit-transform: scale(1.2);
            transform: scale(1.2);
        }
    }

    @media only screen and (max-width: 767px) {

        .nav-home {
            letter-spacing: 0.64px;
            color: #FF0050 !important;
        }

        .desktop-view {
            display: none;
        }

        .hero-image {
            background-image: url("/assets/hero-home.jpg");
            background-color: #cccccc;
            height: 600px;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            position: relative;
            margin-top: -84px;

        }

        .hero-text {
            position: absolute;
            top: 30%;
            margin-left: 10%;
            margin-right: 10%;
            color: white;
        }

        .hero-text h1 {
            font-size:50px
        }

        .text-box {
            margin: auto;
            width: 300px;
        }

        .split-wrap {
            background-color: #171B1E;
        }

        .split.first {
            margin-top: 10%;
            margin-bottom: 15%;
            width: 100%;
            display: block;
            float: left;
            overflow: hidden;
            height: 100%;
            display: flex;
            align-items: center;
            margin-left: 10%;

        }

        .split.second {
            width: 100%;
            display: block;
            float: left;
            overflow: hidden;

            -webkit-transition: -webkit-transform 1s ease;
            transition: -webkit-transform 1s ease;
            transition: transform 1s ease;
            transition: transform 1s ease, -webkit-transform 1s ease;
            max-width: 100%;
            max-height: 100%;
        }

        .split.second img {
            width: 100%;
            height: auto;
            -webkit-transition: -webkit-transform 1s ease;
            transition: -webkit-transform 1s ease;
            transition: transform 1s ease;
            transition: transform 1s ease, -webkit-transform 1s ease;
        }

    }


    .new-range {
        text-align: left;
        font: normal normal normal 16px Proxima Nova;
        letter-spacing: 0.64px;
        color: #FFFFFF;
        text-transform: uppercase;
        opacity: 0.6;
    }

    .car-model {
        text-align: left;
        font: normal normal 800 36px;
        letter-spacing: 0.72px;
        color: #FFFFFF;
        text-transform: uppercase;
        opacity: 0.87;
    }

    .learn-more {
        color: var(--unnamed-color-ff0050);
        text-align: left;
        font: normal normal normal 16px Poppins;
        letter-spacing: 0.64px;
        color: #FF0050;
        opacity: 1;
        margin-top: 20px;
    }

    @font-face {
        font-family: 'proxima_nova_rgregular';
        src: url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.eot');
        src: url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.eot?#iefix') format('embedded-opentype'),
            url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.woff') format('woff'),
            url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.ttf') format('truetype'),
            url('https://litmus.com/fonts/Emails/proximanova-regular-webfont.svg#proxima_nova_rgregular') format('svg');
        font-weight: normal;
        font-style: normal;
    }

    @font-face {
        font-family: 'proxima_nova_rgbold';
        src: url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.eot');
        src: url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.eot?#iefix') format('embedded-opentype'),
            url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.woff') format('woff'),
            url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.ttf') format('truetype'),
            url('https://litmus.com/fonts/Emails/proximanova-bold-webfont.svg#proxima_nova_rgbold') format('svg');
        font-weight: normal;
        font-style: normal;
    }

    @font-face {
        font-family: 'adelle_rgregular';
        src: url('https://litmus.com/fonts/Emails/adelle_reg-webfont.eot');
        src: url('https://litmus.com/fonts/Emails/adelle_reg-webfont.eot?#iefix') format('embedded-opentype'),
            url('https://litmus.com/fonts/Emails/adelle_reg-webfont.woff') format('woff'),
            url('https://litmus.com/fonts/Emails/adelle_reg-webfont.ttf') format('truetype'),
            url('https://litmus.com/fonts/Emails/adelle_reg-webfont.svg#adelle_rgregular') format('svg');
        font-weight: normal;
        font-style: normal;
    }

    body {
        margin: 0;
        font-family: 'proxima_nova_rgregular', Helvetica, Arial, sans-serif;
    }

    h1 {
        font-family: 'proxima_nova_rgbold', Helvetica, Arial, sans-serif;

    }

    p {
        font-family: Poppins;
    }
</style>
