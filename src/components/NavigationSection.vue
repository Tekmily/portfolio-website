<!-- NAVIGATION SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 21, 2022
-->

<template>
<div class="nav">
    <img class="logo" :src="require('@/assets/logo.png')" alt="website logo">

    <!-- <div class="burger-menu">
        <input class="menu-btn" type="checkbox" id="menu-btn" />
        <label class="menu-icon" for="menu-btn"><span class="navicon"></span></label>
    </div> -->
    <div class="menu-container">
        <div class="list-container">
            <ul class="menu" id="menu">
                <li class="item"><a class="link" href="#about-section">ABOUT</a></li>
                <li class="item"><a class="link" href="#webprojects-section">PROJECTS</a></li>
                <li class="item"><a class="link" href="#contact-section">CONTACT</a></li>
            </ul>

            <a id="hamburger" href="#menu" title="menu" class="hamburger">
                <img :src="require('@/assets/burger.png')" alt="">
            </a>
        </div>
        <a href="#!" title="close menu" class="hamburger-close">
            <img :src="require('@/assets/burger-close.png')" alt="">
        </a>
    </div>

</div>
</template>

<style scoped>
*,
*::before,
*::after {
    box-sizing: border-box;
}

body {
    background-color: var(--main-black);
    margin: 0;
    color: white;
}

a {
    text-decoration: none;
}

.menu-container > img {
    max-width: 520px;
}

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    width: 100%;
    background-color: var(--main-black);
    color: white;
    z-index: 5;
    padding: 1rem; 
}

.menu-container {
    position: relative;
}

.hamburger {
    color: inherit;
    min-width: 32px;
    min-height: 32px;
    transition: opacity 80ms linear;
    /* hiding the hamburger icon on large screen sizes */
    display: none;
    opacity: 0;
}

.hamburger-close {
    color: inherit;
    position: absolute;
    top: 0;
    min-width: 32px;
    min-height: 32px;
    transition: opacity 150ms linear;
    /*   hiding the close icon and... */
    display: none;
    opacity: 0;
    z-index: -1; /* pushing it behind the hamburger icon so that hamburger icon can be clicked */
}

.menu {
    padding: 0;
    margin: 0;
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    font-size: 0.95rem;
    font-weight: 500; 
}

.item {
    margin-right: 1em;
}

.link {
    color: white;
    text-decoration: none;
    width: 100%;
    padding: 2vw;
}

.link:hover,
.link:focus-visible {
    box-shadow: 0 4px 0 -1px var(--main-black);
    background-color: var(--main-pink);
    color: white;
}

/* SMALL SCREEN DEVICES */
@media (max-width: 560px) {
    .hamburger {
        /* makes burger visibile to small screens */
        display: flex;
        opacity: 1;
    }

    .menu {
        /*makes menu offscreen */
        opacity: 0;
        position: fixed;
        visibility: none;
        top: -1000px;

        /*styling*/
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: white;
        box-shadow: 0 0 30px rgba(0, 0, 0, 0.19);
        border: 2px solid rgba(255, 255, 255, 0.2); /* part of glass morphism effect */
        border-radius: 2rem 0 2rem 2rem;
        background: var(--main-black);
    }

    .list-container:focus .menu,
    .list-container:focus-within .menu {
        position: absolute;
        visibility: visible;
        opacity: 1;
        top: 2rem;
        right: 1.5rem; 
    }

    @supports (backdrop-filter: blur(10px)) {
        .list-container:focus .menu,
        .list-container:focus-within .menu {
            background: var(--main-black);
            backdrop-filter: blur(10px); 
        }
    }

    .item {
        margin-right: 0;
        padding: 0.5rem 1.5rem;
    }

    .link:hover,
    .link:focus {
        opacity: 0.8;
        color: var(--main-black);
    }

    .list-container:focus .hamburger,
    .list-container:focus-within .hamburger {
        opacity: 0;
        z-index: -1;
    }

    .list-container:focus + .hamburger-close,
    .list-container:focus-within + .hamburger-close {
        display: flex;
        opacity: 1;
        z-index: 1;
    }
}
</style>