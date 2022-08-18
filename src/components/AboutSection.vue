<!-- ABOUT SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 18, 2022
-->
<template>
    <div id="flex-about"> <!-- FLEX LEFT AND RIGHT-->
        <div id="left-side-about"> <!-- FLEX ABOUT AND CERTIFICATIONS-->
            <section>
                <h1 class="global-head1">ABOUT HER</h1>
                <p>She studied Bachelor of Science in Computer Science at the Polytechnic University of the Philippines. She has worked as Content Management System (CMS) Developer & Designer, and has also worked as SEO Specialist since 2018. She excels at designing and developing websites with HTML and CSS.</p>
            </section>
            
<!-- CERTIFICATIONS LIST -->
            <div id="certifications">
                <h3>CERTIFICATIONS</h3>
                <img :src="require('@/assets/web-design-certificate.png')">
                <p><a href="https://freecodecamp.org/certification/fccfefd5801-2c85-4717-a21a-95e74c7cdea5/responsive-web-design" target="_blank">Responsive Web Design</a></p>
            </div>
        </div>

        <div id="right-side-about">
            <img src="./assets/trishia.png" >
        </div>
    </div>
</template>


<style scoped>
.flex-about {
    display: flex;
}

.left-side-about {
    display: flex;
}

</style>
