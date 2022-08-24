<!-- HEADER SECTION WITH ANIMATION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 18, 2022
-->

<template>
    <div class="parallax">
        <div class="content">
            <p>HER NAME IS TRISHIA, AND SHE IS A</p>
            <h1>
                <a href="" class="typewrite" data-period="2000" data-type='[ "WEB DEVELOPER", "FRONTEND DESIGNER", "SEO SPECIALIST", "FRESH GRAD"]'>
                <span class="wrap"></span>
                </a>
            </h1>
            <p class="sub-text">SHE ASPIRES TO CRAFT WEB EXPERIENCES THAT TYPIFY AND INSPIRE.</p>
            <div class="resume">
                <a href="https://drive.google.com/file/d/1ld5Km8hb4-C6Wm4LrAi11UuKwgksfN5K/view?usp=sharing" target="_blank">DOWNLOAD RESUME</a>
            </div>
        </div>
    </div>
</template>

<script>
var TxtType = function(el, toRotate, period) {
        this.toRotate = toRotate;
        this.el = el;
        this.loopNum = 0;
        this.period = parseInt(period, 10) || 2000;
        this.txt = '';
        this.tick();
        this.isDeleting = false;
    };

    TxtType.prototype.tick = function() {
        var i = this.loopNum % this.toRotate.length;
        var fullTxt = this.toRotate[i];

        if (this.isDeleting) {
        this.txt = fullTxt.substring(0, this.txt.length - 1);
        } else {
        this.txt = fullTxt.substring(0, this.txt.length + 1);
        }

        this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

        var that = this;
        var delta = 200 - Math.random() * 100;

        if (this.isDeleting) { delta /= 2; }

        if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
        } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
        }

        setTimeout(function() {
        that.tick();
        }, delta);
    };

    window.onload = function() {
        var elements = document.getElementsByClassName('typewrite');
        for (var i=0; i<elements.length; i++) {
            var toRotate = elements[i].getAttribute('data-type');
            var period = elements[i].getAttribute('data-period');
            if (toRotate) {
              new TxtType(elements[i], JSON.parse(toRotate), period);
            }
        }
        // INJECT CSS
        var css = document.createElement("style");
        css.type = "text/css";
        css.innerHTML = ".typewrite > .wrap { border-right: 0.08em solid #fff}";
        document.body.appendChild(css);
    };
</script>

<style scoped>
.parallax {
    background-image: url("@/assets/background-head.png");
    min-height: 720px;
    width: 100%;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.content {
    height: 100%;
    text-align: center;
    color:#fff;
    padding-top:7em;
}

* { 
    color:#fff; text-decoration: none;
}

.typewrite {
    background-color: var(--main-pink);
    color: white;
    padding: 1vw;
    font-size: 64px;
}

.content p {
    font-size: 24px;
}

.sub-text {
    padding: 2vw;
    font-size: 32px;
}

.resume {
    width: clamp(150px, 30%, 250px);
    height: clamp(50px, 20%, 100px);
    border: 2px solid white;
    margin: auto;
    padding: 1vw;
    font-size: 20px;
}

.resume:hover {
    background-color: var(--main-pink);
    color: white;
}
</style>