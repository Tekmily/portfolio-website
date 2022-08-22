<!-- CONTACT SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 18, 2022
-->

<template>
    <div class="contact-area">
        <div class="contact-info">
            <h3 class="title">CONTACT DETAILS</h3>
            <div class="single-contact">
                <div class="icon">
                    <img :src="require('@/assets/logos/email.png')" alt=""></div>
                <div class="details">
                    <h4><a class="single-link" href="mailto:trishiacabuang.work@gmail.com">trishiacabuang.work@gmail.com</a></h4>
                </div>
            </div>

            <div class="single-contact">
                <div class="icon">
                    <img :src="require('@/assets/logos/phone.png')" alt=""></div>
                <div class="details">
                    <h4><a class="single-link" href="tel:09954532395">0995 453 2395</a></h4>
                </div>
            </div>

            <div class="single-contact">
                <div class="icon">
                    <img :src="require('@/assets/logos/map.png')" alt=""></div>
                <div class="details">
                    <h4>Pasay City, Philippines</h4>
                </div>
            </div>
        </div>

        <div class="contact-schedule">
            <h3 class="title">SCHEDULE</h3>
            <!-- <div class="sched-list"> -->
                <p class="sched-list">Mon to Fri 9AM to 6PM</p>
                <p class="sched-list">Sat & Sun 10AM to 5PM</p>
            <!-- </div> -->
            <div id="profiles">
                <a href="https://www.linkedin.com/in/trishia-ann-cabuang/"><img class="social-icon" :src="require('@/assets/logos/LinkedIn.png')" alt="LinkedIn"></a>
                <a href="https://www.monster.com.ph/seeker/dashboard?resume=true"><img class="social-icon" :src="require('@/assets/logos/Monster.png')" alt="Monster"></a>
                <a href="https://github.com/devtagcabuang"><img class="social-icon" :src="require('@/assets/logos/Github.png')" alt="Github"></a>
                <a href="https://my.indeed.com/resume?hl=en&co=PH&from=gnav-resume--myind"><img class="social-icon" :src="require('@/assets/logos/Indeed.png')" alt="Indeed"></a>
                <a href="https://myjobstreet.jobstreet.com.ph/resume/preview-resume.php?x=a02lo58v9dg6g5in8dei478gn7"><img class="social-icon" :src="require('@/assets/logos/Jobstreet.png')" alt="Jobstreet"></a>
            </div>
        </div>
    </div>
    <footer>
        <p>Built by Trishia Ann Cabuang ⓒ 2022</p>
    </footer>
</template>

<style scoped>

footer p {
    font-size: 16px;
    background-color: var(--main-pink);
    color: var(--main-black);
}

.contact-area {
    display: flex;
    justify-content: space-evenly;
    align-content: center;
    gap: 10%;
    flex-wrap: wrap;
    padding-top: 0;
    padding-bottom: 20px;
    position: relative;

}
/* .contact-info {
    display: flex;
    flex-direction: column;
    width: 40%;
} */

.single-contact {
    display: block;
    text-align: left;
}

.title {
    text-align: left;
}

.single-contact .icon {
    display: inline-block;
    text-align: left;
    vertical-align: middle;
    margin-left: 15px;
    line-height: 2em;
}

.single-contact .details {
    display: inline-block;
    text-align: left;
    vertical-align: middle;
    margin-left: 15px;
}

.details .single-link {
    color: var(--main-gray);
    text-decoration: none;
    font-size: 20px;
    font-weight: normal;
}

.details h4 {
    color: var(--main-gray);
    font-size: 20px;
    font-weight: normal;
}

.contact-schedule .sched-list {
    display: block;
    text-align: left;
    margin-left: 15px;
}

#profiles {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    padding-top: 2vw;
}

#profiles .social-icon {
    margin-right: 10px;
	-webkit-transform: scale(1);
	transform: scale(1);
	-webkit-transition: .3s ease-in-out;
	transition: .3s ease-in-out;
}

#profiles .social-icon:hover {
	-webkit-transform: scale(1.3);
	transform: scale(1.3);
}

</style>