<template>
    <!-- Navigation bar -->
    <header class="header">
        <!-- Logo -->
        <img class="header-item header-logo" :src="require(`~/assets/logo.svg`)" />
        <!-- Hamburger icon -->
        <input class="side-menu" type="checkbox" id="side-menu"/>
        <label class="hamb" for="side-menu"><span id="hamb-line" class="hamb-line"></span></label>
        <!-- Menu -->
        <nav class="nav">
            <ul class="menu">
                <li class="close-menu-li"><a><span class="close-menu" onclick="document.getElementById('hamb-line').click()">x</span></a></li>
                <li><a class="mobile-menu-head">MENU</a></li>
                <li><a id="nav-home" class="nav-item nav-home" href="/">HOME</a></li>
                <li><a id="nav-contact" class="nav-item nav-contact" href="/contact">CONTACT US</a></li>
            </ul>
        </nav>
    </header>

</template>

<script>
export default {
  name: "AppHeader"
};

</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins');

    .header-logo {
        margin-left: 80px;
        margin-top: 30px;
    }

    .nav-item {

        text-align: left;
        font-size: 16px;
        font-family: 'proxima_nova', Helvetica, Arial, sans-serif;
        letter-spacing: 0.64px;
        color: #FFFFFF;
        text-transform: uppercase;
        opacity: 0.6;
    }

    /* Header */
    .header {
        background-color: var(--black);
        box-shadow: 1px 1px 5px 0px var(--gray);
        position: sticky;
        top: 0;
        width: 100%;
        z-index: 9999;
    }

    /* Logo */
    .logo {
        display: inline-block;
        color: #ffffff;
        font-size: 60px;
        margin-left: 10px;
    }

    /* Nav menu */
    .nav {
        width: 100%;
        height: 100%;
        position: fixed;
        overflow: hidden;

    }

    .menu a:hover {
        color: #ffffff;
        opacity: 0.6;
    }

    .nav {
        max-height: 0;
        transition: max-height .5s ease-out;
    }

    /* Menu Icon */
    .hamb {
        cursor: pointer;
        float: right;
        padding: 40px 20px;
        color: #ffffff;
    }

    /* Style label tag */

    .hamb-line {
        background: #ffffff;
        display: block;
        height: 2px;
        position: relative;
        width: 24px;
    }

    /* Style span tag */

    .hamb-line::before,
    .hamb-line::after {
        background: #ffffff;
        content: '';
        display: block;
        height: 100%;
        position: absolute;
        transition: all .2s ease-out;
        width: 100%;
    }

    .hamb-line::before {
        top: 5px;
    }

    .hamb-line::after {
        top: -5px;
    }

    .side-menu {
        display: none;
    }

    /* Hide checkbox */


    /* Toggle menu icon */
    .side-menu:checked~nav {
        max-height: 100%;
    }

    .side-menu:checked~.hamb .hamb-line {
        background: transparent;
    }

    .side-menu:checked~.hamb .hamb-line::before {
        transform: rotate(-45deg);
        top: 0;
    }

    .side-menu:checked~.hamb .hamb-line::after {
        transform: rotate(45deg);
        top: 0;
    }

    /* Responsiveness */
    @media (min-width: 768px) {
        .nav {
            max-height: none;
            top: 0;
            position: relative;
            float: right;
            width: fit-content;
        }

        .menu li {
            float: left;
        }

        .menu a:hover {
            background-color: transparent;
            color: #ffffff;
            opacity: 0.6;

        }

        .menu a {
            display: block;
            padding: 30px;
            color: #ffffff;
        }

        .hamb {
            display: none;
        }

        .close-menu {
            display: none !important;
        }

        .mobile-menu-head {
            display: none !important;
        }
    }

    /* Responsiveness */
    @media (max-width: 767px) {
        .close-menu-li {
            height: 60px;
        }

        .close-menu-li a {}

        .nav {
            margin-top: -46px;
            background-color: #171B1E;
        }

        .close-menu {
            float: right;
            margin-right: 15px;
            font-size: 30px;
            color: #ffffff;
        }

        .mobile-menu-head {
            text-align: left;
            font-size: 24px;
            font-family: 'proxima_nova', Helvetica, Arial, sans-serif;
            letter-spacing: 0.48px;
            color: #FFFFFF;
            text-transform: uppercase;
            opacity: 0.87;
            font-weight: bold;
            padding-bottom: 20px;
        }

        .menu {
            width: 100%;
        }

        .menu a {
            display: block;
            padding: 5px;
            color: #ffffff;
        }
    }
</style>
