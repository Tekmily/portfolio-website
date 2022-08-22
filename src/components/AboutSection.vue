<!-- ABOUT SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 18, 2022
-->
<template>
    <div id="flex-about"> <!-- FLEX LEFT AND RIGHT-->
        <div class="grid-container">
            <div id="left-about"> <!-- FLEX ABOUT AND CERTIFICATIONS-->
                <section class="about-info">
                    <h1>ABOUT HER</h1>
                    <p>She studied Bachelor of Science in Computer Science at the Polytechnic University of the Philippines. She has worked as Content Management System (CMS) Developer & Designer, and has also worked as SEO Specialist since 2018. She excels at designing and developing websites with HTML and CSS.</p>
                </section>
                <!-- CERTIFICATIONS LIST -->
                <section id="certifications">
                    <h3>CERTIFICATIONS</h3>
                        <div class="cert-info">
                            <img class="qr-image" :src="require('@/assets/web-design-certificate.png')">
                            <p class="cert-title"><a href="https://freecodecamp.org/certification/fccfefd5801-2c85-4717-a21a-95e74c7cdea5/responsive-web-design" target="_blank">Responsive Web Design</a></p>
                        </div>
                </section>
            </div>
                <!-- PHOTO -->
            <div id="right-about">
                <img class="my-image" :src="require('@/assets/trishia.png')" >
            </div>
        </div>
    </div>
</template>


<style scoped>

*,
::before,
::after {
    padding: 0;
    margin: 0;
}

html {
    box-sizing: border-box;
}

.flex-about {
    display: grid;
    grid-template-columns:
        minmax(3rem, 1fr)
        minmax(min-content, 94rem)
        minmax(3rem, 1fr);
    row-gap: 2rem;
}

.grid-container {
    display: grid;
    grid-template-columns: 2fr 1fr;
    column-gap: 3rem;
    margin-bottom: 3rem;
    padding: 8vh;
    place-items: center;
}

.about-info {
    margin-bottom: 5vh;
    margin-left: 5vh;
    text-align: left;
}

/* MISC */

.my-image {
    width: clamp(350px, 25%, 760px);
    height: clamp(450px, 30%, 960px);
    margin-right: 5vh;
}


.cert-info .qr-image {
    width: clamp(64px, 25%, 150px);
    height: clamp(64px, 30%, 150px);
    align-items: left;
}

.cert-title a {
    color: var(--main-gray);
    text-decoration: none;
    font-size: 20px;
}

#certifications {
    margin-bottom: 3vh;
    margin-left: 5vh;
    text-align: left;
}
/* MEDIA QUERY */
@media only screen and (max-width: 920px) {
    .grid-container {
        grid-template-columns: 1fr;
    }

    #certifications {
        margin-bottom: 3vh;
        text-align: center;
        margin-left: 0;
    }

    .cert-title {
        text-align: center;
    }

    .about-info {
        text-align: center;
        margin-left: 0;
    }

    .my-image {
        margin-right: 0;
    }
}
</style>
