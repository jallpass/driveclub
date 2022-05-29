<template>
    <div>
        <div class="hero-image" style="border-bottom: 1px solid #ffffff;">
            <div class="hero-text">
                <h1 style="font-size:50px">{{ heroTitle }}</h1>
                <h3>24/7 SUPPORT</h3>
            </div>
        </div>
        <div class="floating-contact-box">
            <div class="inner-contact-box m-5">
                <h3 class="form-header">HOW CAN WE HELP?</h3>
                <form action="/action_page.php">
                    <label for="name">Name</label>
                    <input type="text" id="name" name="name" class="w-100 mb-2">
                    <label for="contact_number">Contact number</label>
                    <input type="text" id="contact_number" name="contact_number" class="w-100 mb-2">
                    <label for="email">Email address</label>
                    <input type="email" id="email" name="email"  class="w-100 mb-2">
                    <label for="info">How can we help?</label>
                    <textarea id="info" name="info"  class="w-100 mb-2" rows="5"></textarea>
                    <button type="submit" class="form-btn">Submit</button>
                </form>
            </div>
        </div>
        <!-- new div -->
        <div style="background-color: #171B1E;" class="split-wrap">
            <div class="cover">
                <div class="text-block">
                    <div class="icon-box phone-icon-box">
                        <img class="phone-icon" :src="require(`~/assets/phone.svg`)" />
                    </div>
                    <div class="text-box">
                        <div class="text-header">Phone</div>
                        <div class="text-detail">082 000 0000</div>
                    </div>
                </div>
                <div class="text-block">
                    <div class="icon-box envelope-icon-box">
                        <img class="envelope-icon" :src="require(`~/assets/envelope.svg`)" />
                    </div>
                    <div class="text-box">
                        <div class="text-header">Email</div>
                        <div class="text-detail">email@example.com</div>
                    </div>
                </div>
                <div class="text-block">
                    <div class="icon-box location-icon-box">
                        <img class="location-icon" :src="require(`~/assets/location.svg`)" />
                    </div>
                    <div class="text-box">
                        <div class="text-header">Location</div>
                        <div class="text-detail">42 Business Rd</div>
                    </div>
                </div>
            </div>
        </div>
        <!-- new div -->
        <div style="background-color: #171B1E;" class="split-wrap split-wrap-2">
        </div>
    </div>
</template>

<script>
    export default {
        head() {
            return {
                title: "Contact Us",
                meta: [
                    {
                        hid: "description",
                        name: "description",
                        content: "contact us page"
                    }
                ]
            };
        },
        data() {
            return {
                heroTitle: "CONTACT US"
            }
        }
    };

</script>

<style>
    .form-btn {
        background: rgba(255, 0, 80, 0.30196) 0% 0% no-repeat padding-box;
        border: 2px solid #FF0050;
        opacity: 1;
        font-size: 14px;
        color: #FFFFFF;
        padding: 4px 20px 4px 20px;
    }


    .floating-contact-box label {
        text-align: left;
        font: normal normal medium 14px/18px Montserrat;
        letter-spacing: 0px;
        color: #FFFFFF;
        opacity: 0.87;
        display: block;
    }

    .floating-contact-box input {
        background-color: #171B1E;
        border: 1px solid #FFFFFFDE;
        display: block;
    }

    .floating-contact-box textarea {
        background-color: #171B1E;
        border: 1px solid #FFFFFFDE;
    }

    .form-header {
        text-align: left;
        font-weight: bold;
        font-size: 32px;
        font-family: 'proxima_nova', Helvetica, Arial, sans-serif;
        letter-spacing: 1.28px;
        color: #FFFFFF;
        text-transform: uppercase;
        opacity: 0.87;
    }

    .cover {
        margin-top: 60px;
        margin-bottom: 60px;
        margin-left: 100px;
    }

    .text-block {
        margin-top: 10px;
        margin-bottom: 10px;
    }

    .icon-box {
        margin-right: 20px;
    }

    .text-header {
        text-align: left;
        font: normal normal medium 18px/21px Poppins;
        letter-spacing: 0.36px;
        color: #FFFFFF;
        opacity: 0.87;
    }

    .text-detail {
        text-align: left;
        font: normal normal 300 18px/21px Poppins;
        letter-spacing: 0.36px;
        color: #FFFFFF;
        opacity: 0.6;
    }

    .phone-icon-box {
        width: 42px;
        background: #FF00504D 0% 0% no-repeat padding-box;
        border: 2px solid #FF0050;
        opacity: 1;
        float: left;
    }

    .envelope-icon-box {
        width: 42px;
        background: #FF00504D 0% 0% no-repeat padding-box;
        border: 2px solid #FF0050;
        opacity: 1;
        float: left;
    }

    .location-icon-box {
        width: 42px;
        background: #FF00504D 0% 0% no-repeat padding-box;
        border: 2px solid #FF0050;
        opacity: 1;
        float: left;
    }

    .phone-icon {
        width: 20px;
        fill: white;
        margin: 10px;
    }

    .envelope-icon {
        width: 19px;
        fill: white;
        margin: 10px;
    }

    .location-icon {
        width: 16px;
        fill: white;
        margin: 9px;
        margin-left: 10px;
    }

    @media only screen and (min-width: 768px) {
        .nav-contact {
            text-align: center;
            letter-spacing: 0.64px;
            color: #FF0050 !important;
            opacity: 1;
            border-top: 3px solid #FF0050;
        }

        .hero-image {
            background-image: url("/assets/hero-contact.jpg");
            background-color: #cccccc;
            height: 600px;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            position: relative;
            margin-top: -84px;
        }

        .split-wrap-2 {
            height: 250px;
            border-top: 1px solid rgb(255, 255, 255);
        }

        .hero-text {
            position: absolute;
            top: 200px;
            left: 100px;
            color: white;
        }
    }

    @media only screen and (min-width: 951px) {
        .split-wrap-2 {
            height: 250px;
            border-top: 1px solid rgb(255, 255, 255);
        }

        .floating-contact-box {
            border: 1px solid #ffffff;
            display: inline-block;
            position: absolute;
            top: 510px;
            right: 10%;
            background-color: #171B1E;
            z-index: 9999;
        }
    }

    @media only screen and (min-width: 767px) and (max-width: 950px) {
        .hero-image {
            background-image: url("/assets/hero-contact.jpg");
            background-color: #cccccc;
            height: 600px;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            position: relative;
            margin-top: -84px;

        }

        .split-wrap-2 {
            display: none;
        }

        .hero-text {
            position: absolute;
            top: 200px;
            left: 100px;
            color: white;
        }

        .floating-contact-box {
            border-top: 1px solid #ffffff;
            border-bottom: 1px solid #ffffff;
            display: block;
            background-color: #171B1E;
        }

        .cover {
            margin-left: 5% !important;
        }

        .inner-contact-box {
            margin-left: 5% !important;
            margin-right: 5% !important;
        }

    }

    @media only screen and (max-width: 767px) {
        .nav-contact {
            letter-spacing: 0.64px;
            color: #FF0050 !important;
        }

        .split-wrap-2 {
            display: none;
        }

        .floating-contact-box {
            border-top: 1px solid #ffffff;
            border-bottom: 1px solid #ffffff;
            display: block;
            background-color: #171B1E;
        }

        .hero-image {
            background-image: url("/assets/hero-contact.jpg");
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

        .cover {
            margin-left: 5% !important;
        }

        .inner-contact-box {
            margin-left: 5% !important;
            margin-right: 5% !important;
        }
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
