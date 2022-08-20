<!-- NAVIGATION SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 18, 2022
-->
<template>
    <div id="nav-head">
        <!-- LOGO -->
        <div id="logo">
            <img :src="require('@/assets/logo.png')" alt="website logo">
        </div>

        <!-- NAVIGATION MENU -->
            <!-- CHECKBOX -->
            <input type="checkbox" id="nav-checbox" class="nav-checkbox">
            <label for="nav-checkbox" class="nav-toggle">
                <img class="menu" :src="require('@/assets/burger.png')" alt="burger icon">
                <img class="close" :src="require('@/assets/burger-close.png')" alt="burger close icon">
            </label>

            <!-- NAV CONTENT -->
        <ul class="nav-menu">
            <div class="nav-menu">
                <li><a href="#about-section">ABOUT</a></li>
                <li><a href="#webprojects-section">PROJECTS</a></li>
                <li><a href="#contact-section">CONTACT</a></li>
            </div>

            <!-- <div class="phone-menu">
                <li><a href="#about-section">ABOUT</a></li>
                <li><a href="#webprojects-section">PROJECTS</a></li>
                <li><a href="#contact-section">CONTACT</a></li>
            </div> -->
        </ul>
    </div>

</template>

<script setup>
</script>

<style scoped>
*,
*::before,
*::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    color: var(--main-gray);
    font-size: 18px;
    height: 100vh;
}

.nav-toggle {
    position: absolute;
    cursor: pointer;
    margin: 0rem 1rem;
    right: 0;
}

.close {
    display: none;
}

.menu {
    margin-top: 0.2rem;
}

.nav-checkbox {
    display: none;
}

.nav-menu {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    align-items: center;
    margin: 1rem;
}

.nav-menu li {
    list-style: none;
    display: none;
}

.nav-menu li :first-child {
        margin-right: auto;
        display: block;
}

a {
    text-decoration: none;
    color: white;
    font-size: 18px;
}

/* TOGGLE THE BURGER */
#nav-checkbox:checked ~ ul.nav-menu li {
    display: block;
}

/* CHANGE MENU TO CLOSE  */
#nav-checkbox:checked ~ label.nav-toggle .close {
    display: block;
}

#nav-checkbox:checked ~ label.nav-toggle {
    display: none;
}

/* DESKTOP VIEW  */
@media only screen and (min-width: 560px) {
    .nav-toggle {
        display: none;
    }

    .nav-menu {
        flex-direction: row;
    }

    .nav-menu li {
        display: block;
    }
}
</style>