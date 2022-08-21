<!-- ACTIVE WEBSITES HANDLED SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 18, 2022
-->

<template>
    <div class="quote">
        <blockquote class="web-blockquote">
            <h2>Well, there's more!
            <p>Aside from the notable websites mentioned above, she also designed, developed, and managed over forty websites while freelancing and working part-time while pursuing a Bachelor of Science in Computer Science at PUP.</p>
            </h2>
        </blockquote>
    </div>

    <div class="web-list">
        <div class="other-active">
            <h3 class="head-format">ACTIVE WEBSITES</h3>
            <p class="para-format">The websites listed below are all currently operational and have been managed by her in the most recent few years. Some of them are personal blog networks, while others are client websites.</p>
            <ul>
                <li>Roofing Waterloo</li>
                <li>WNY Websites</li>
                <li>Arc Web Soln's</li>
                <li>B2B Online</li>
                <li>Price Foundation</li>
                <li>The Harpers</li>
            </ul>
        </div>

        <div class="other-active">
            <h3 class="head-format">ALL DOMAIN</h3>
            <p class="para-format">She kept track of all the domain names she worked on for various clients and private blog networks in Excel. She was also in charge of domain registration, hosting (via hosting services), and website maintenance. Some of the domains have already been removed, and others have been sold. That being said, you can view the domain's documentation and check the domains she managed by clicking the buttons below.</p>
        </div>
    </div>
<!-- BUTTONS -->
    <div class="web-buttons">
        <div class="web-docubutton">
            <a href="https://drive.google.com/drive/folders/1CC36ZCIcS0v3sSNVu0JqO5kpdcPQ4A3X?usp=sharing">DOCUMENTATION</a>
        </div>

        <div class="web-listbutton">
            <a href="https://drive.google.com/drive/folders/1CC36ZCIcS0v3sSNVu0JqO5kpdcPQ4A3X?usp=sharing">FULL LIST</a>
        </div>
    </div>
</template>

<style scoped>
.quote {
    margin-left: -4vw;
    margin-right: 5vw;
    margin-top: 2vw
}

blockquote {
    display: block;
    background: transparent;
    width: 90%;
    height: 30%;
    padding: 10px 15px 10px 30px;
    /* margin-left: ; */
    position: relative;
/* FONT */
    font-family: inherit;
    font-size: 24px;
    line-height: 1.2;
/* BORDERS  */
    border-left-style: solid;
    border-left-width: 15px; 
    border-left-color: var(--main-pink);
}

blockquote::before {
    content: "\201C";
    font-family: Georgia, serif;
    font-size: 60px;
    font-weight: bold;
    color: #999;
    position: absolute;
    left: 10px;
    top:5px;
}

blockquote::after {
    content: "";
}

h2 {
    text-align: left;
    font-size: 28px;
}

.web-blockquote p {
    font-size: 20px;
    color: var(--main-gray);
    font-weight: normal;
}

/* BUTTON  */
.web-docubutton {
    width: clamp(150px, 30%, 250px);
    height: clamp(50px, 20%, 100px);
    border: 2px solid white;
    margin: auto;
    padding: 1vw;
    font-size: 20px;
}

.web-docubutton:hover {
    background-color: var(--main-pink);
    color: white;
}

.web-docubutton a {
    text-decoration: none;
    color: white;
}
</style>