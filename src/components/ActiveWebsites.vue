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
                <li><a href="http://www.ankitasadani.com/" target="_blank">WNY Website</a></li>
                <li><a href="https://roofingwaterloo.com/" target="_blank">Roofing Waterloo</a></li>
                <li><a href="http://arcwebsolutions.net/" target="_blank">Arc Web Soln's</a></li>
                <li><a href="http://www.b2buniversityonline.com/" target="_blank">B2B Online</a></li>
                <li><a href="http://www.thepricefoundation.com" target="_blank">Price Foundation</a></li>
                <li><a href="http://www.gulfcoastharpers.org/" target="_blank">The Harpers</a></li>
            </ul>
            <div class="web-docubutton">
                <a href="#webprojects-section">NOTABLE WEBSITES</a>
            </div>
        </div>

        <div class="other-active">
            <h3 class="head-format">ALL DOMAINS</h3>
            <p class="para-format">She kept track of all the domain names she worked on for various clients and private blog networks in Excel. She was also in charge of domain registration, hosting (via hosting services), and website maintenance. Some of the domains have already been removed, and others have been sold. That being said, you can view the domain's documentation and check the domains she managed by clicking the buttons below.</p>

            <!-- BUTTONS -->
            <div class="web-buttons">
                <div class="web-docubutton">
                <a href="https://drive.google.com/drive/folders/1CC36ZCIcS0v3sSNVu0JqO5kpdcPQ4A3X?usp=sharing">DOCUMENTATION</a>
                </div>

                <div class="web-docubutton">
                <a href="https://drive.google.com/drive/folders/1CC36ZCIcS0v3sSNVu0JqO5kpdcPQ4A3X?usp=sharing">FULL LIST</a>
                </div>
            </div>
        </div>
    </div>

</template>

<style scoped>
/* BUTTON  */
.web-buttons {
    display: flex;
    justify-content: center;
    align-items: start;
    gap: 20px;
    flex-wrap: wrap;
    margin: 0;
    padding: 0;
}
.web-docubutton {
    width: clamp(150px, 30%, 250px);
    height: clamp(50px, 20%, 100px);
    border: 2px solid var(--main-black);
    margin: auto;
    padding: 1vw;
    font-size: 18px;
}

.web-docubutton:hover {
    background-color: var(--main-pink);
    color: white;
}

.web-docubutton a {
    text-decoration: none;
    color: white;
}

/* CARDS */
.web-list {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    gap: 20px;
    flex-wrap: wrap;
}

.other-active {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: var(--main-gray);
    width: clamp(100px, 50%, 550px);
    height: clamp(450px, 40%, 1200px);
    position: relative;
    border-radius: 4px;
    padding: 20px;
}

.other-active > * {
    padding: 10px;
}

.other-active:hover {
    background: var(--sub-pink);
    color: #fff;
    box-shadow: 0px 0px 11px 5px #000000;
}

.head-format {
    color: var(--main-pink);
	font-weight: 900;
	letter-spacing: 2px;
	text-transform: uppercase;
	font-size: 32px;
    text-shadow: 1px 0px 2px black;
	white-space: wrap;
    overflow: hidden;
    text-overflow: ellipsis;
    padding: 0;
    margin-bottom: 1vw;
}

.para-format {
    font-size: 18px;
	line-height: 24px;
	color: var(--main-black);
}

.other-active ul {
    padding-top: 0;
}
.other-active li {
    list-style: none;
}

.other-active a {
    text-decoration: none;
    color: var(--main-black);
    font-size: 16px;
}

.other-active a:hover {
    color: white;
}
/* FOR BLOCKQUOTE  */
.quote {
    margin-left: 1vw;
    margin-right: 5vw;
    margin-top: 2vw;
    margin-bottom: 2vw;
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


</style>