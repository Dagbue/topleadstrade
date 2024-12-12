<template>
  <div class="alpha">
    <main>
      <h1>Testimonials</h1>

      <p class="text-1">What our Customers Say.</p>

      <!-- 01. Emma -->
<!--      <section class="t-bq-section" id="emma">-->
<!--        <div class="t-bq-wrapper t-bq-wrapper-boxed">-->
<!--          <div class="t-bq-quote t-bq-quote-emma">-->
<!--            <div class="t-bq-quote-emma-qmark"><span>&#10077;</span></div>-->
<!--            <div class="t-bq-quote-emma-userpic"></div>-->
<!--            <div class="t-bq-quote-emma-base">-->
<!--              <blockquote class="t-bq-quote-emma-text" cite="Strugatsky brothers">-->
<!--                Deeds are to be worshipped, not statues. And maybe even deeds do not need to be worshipped. Because everyone does what he can. One is for a revolution, the other is for a penny whistle. Maybe I only have enough strength for one penny whistle, so what am I now, a piece of shit?...-->
<!--              </blockquote>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->
<!--      </section>-->









      <!-- 02. Sophia -->
<!--      <section class="t-bq-section" id="sophia">-->
<!--        <div class="t-bq-wrapper t-bq-wrapper-boxed">-->
<!--          <div class="t-bq-quote t-bq-quote-sophia">-->
<!--            <div class="t-bq-quote-sophia-base">-->
<!--              <blockquote class="t-bq-quote-sophia-text" cite="Братья Стругацкие">-->
<!--                And the child meekly looks at you and thinks: you, of course, are an adult, hefty, you can flog me, however, as you have been a fool since childhood, you remain it now, and you will die fool, but this is not enough for you, you want to turn me into a fool as well...-->
<!--              </blockquote>-->
<!--            </div>-->
<!--            <div class="t-bq-quote-sophia-author"><cite>Strugatsky brothers</cite></div>-->
<!--            <div class="t-bq-quote-sophia-userpic"></div>-->
<!--          </div>-->
<!--        </div>-->
<!--      </section>-->









      <!-- 03. Jenny -->

      <div class="slider">

        <section
            v-for="(testimonial, index) in testimonials"
            :key="testimonial.id"
            class="t-bq-section"
            v-show="currentTestimonialIndex === index"
            :class="{ 'fade-in': currentTestimonialIndex === index }"
        >
          <div class="t-bq-wrapper t-bq-wrapper-boxed">
            <div class="t-bq-quote t-bq-quote-jenny">
              <div class="t-bq-quote-jenny-base">
                <blockquote class="t-bq-quote-jenny-text" :cite="testimonial.cite">
                  {{ testimonial.text }}
                </blockquote>
              </div>
              <div class="t-bq-quote-jenny-meta">
                <div class="t-bq-quote-jenny-meta-info">
                  <div class="t-bq-quote-jenny-author">
                    <cite>{{ testimonial.author }}</cite>
                  </div>
                  <div class="t-bq-quote-jenny-source">
                    <span>{{ testimonial.source }}</span>
                  </div>
                </div>
                <div class="t-bq-quote-jenny-userpic">
                  <img :src="testimonial.image" alt="image" class="t-bq-quote-jenny-userpic" />
                </div>
              </div>
            </div>
          </div>
        </section>
      </div>


    </main>
  </div>
</template>



<script>
export default {
  name: "HomeSection7",
  data() {
    return {
      currentTestimonialIndex: 0,
      testimonials: [
        {
          id: 1,
          text: "TopLeads Trade has created a quality platform for trading cryptocurrency derivatives. We were most impressed " +
              "by the exchange’s design and overall user experience, which is truly first-class.",
          author: "Emma Avon",
          source: "Investor",
          cite: "Emma Avon",
          image: "https://margex.com/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fuser_avatar.8b1c8174.png&w=128&q=75"
        },
        {
          id: 2,
          text: "TopLeads Trade is gradually taking over the crypto,Forex,and stocks derivatives market through its " +
              "unique and user-friendly platform.",
          author: "Casper Brown",
          source: "Trader",
          cite: "Casper Brown",
          image: "https://img.freepik.com/free-photo/young-bearded-man-with-striped-shirt_273609-5677.jpg?t=st=1716809930~exp=1716813530~hmac=6212a4af3b0d29b1a6173cc70811fbfad908c61e46a1a64ab3bc04dc9e218c9a&w=1800"
        },
        {
          id: 3,
          text: "TopLeads Trade is a true refreshment in the crypto derivatives space. The platform offers low fees, high " +
              "leverage and security standards.",
          author: "Rene Peters",
          source: "Doctor",
          cite: "Rene Peters",
          image: "https://img.freepik.com/free-photo/excited-beautiful-young-woman-smiling-hopeful-camera_176420-30191.jpg?t=st=1716809852~exp=1716813452~hmac=23b179822342af63c7940370f896dfb2df342678a6b71cbea725e4849fb69849&w=1800"
        },
        {
          id: 4,
          text: "TopLeads Trade is a solid broker for beginners that want to learn how to trade with leverage." +
              " There are no complicated features or distractions.",
          author: "Kevin",
          source: "Student",
          cite: "Kevin",
          image: "https://img.freepik.com/free-photo/portrait-hispanic-college-student-carrying-backpack-standing-school-hallway_662251-1109.jpg?t=st=1716809973~exp=1716813573~hmac=27d9a285461ac02cd6cae91b6bcb73f9d93cced3288e25af3afeed6917cc8635&w=1060"
        },
        // Add other testimonials here
      ],
      slideInterval: null
    };
  },
  created() {
    this.startSlideshow();
  },
  beforeDestroy() {
    this.stopSlideshow();
  },
  methods: {
    startSlideshow() {
      this.slideInterval = setInterval(() => {
        this.currentTestimonialIndex = (this.currentTestimonialIndex + 1) % this.testimonials.length;
      }, 5000); // Change slide every 3000 ms (5 seconds)
    },
    stopSlideshow() {
      clearInterval(this.slideInterval);
    }
  }
}
</script>


<style scoped>



main {
  /*width: 800px;*/
  display: block;
  margin-left: auto;
  margin-right: auto;

  padding-top: 7%;
  padding-bottom: 7%;
  /*background: #f4f5f6;*/

  background-image: url("@/assets/leaf-bg.svg");
  /*background-color: #000;*/
  height: 100%;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  /*padding-bottom: 10%;*/
}

.alpha{
  height: 100%;
}

main h1 {
  text-align: center;
  font-size: clamp(2rem, 4vw, 2.4rem);
  color: #000000;
  font-family: 'BR-Firma-Bold', sans-serif;
}

.text-1 {
  font-size: 18px;
  line-height: 24px;
  letter-spacing: -0.015em;
  text-align: center;
  color: #697582;
  margin-bottom: 24px;
}




* {
  box-sizing: border-box;
  outline: 0;
  transition: all 0.3s ease;
}

body {
  margin: 0;
  margin-top: 60px;
  padding: 0;
  line-height: 1.68em;
  color: #333333;
  background: #fafafa;
}

blockquote {
  padding: 0;
  margin: 0;
}

section.t-bq-section {
  padding: 30px;
  margin-bottom: 60px;
}

.t-bq-wrapper.t-bq-wrapper-boxed {
  max-width: 800px;
  margin: 0 auto;
}

.t-bq-wrapper.t-bq-wrapper-fullwidth {
  max-width: 100%;
}

.t-bq-wrapper .t-bq-quote {
  padding: 20px;
}


.fade-in {
  animation: fadeIn 1s;
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Additional styling for smoother fading */
.t-bq-section {
  position: absolute;
  width: 100%;
}
.slider {
  position: relative;
  height: 300px; /* Set this to the height of your testimonials or as needed */
}







/* ========== 01. Emma ========== */

.t-bq-quote-emma {
  position: relative;
  display: flex;
  flex-direction: row;
  min-height: 250px;
  background: #ffffff;
  padding: 0!important;
  align-items: stretch;
  border-radius: 20px;
  box-shadow: 2px 2px 25px #cecece;
}

.t-bq-quote-emma .t-bq-quote-emma-qmark {
  position: absolute;
  top: -30px;
  left: calc(50% - 30px);
  background: #ffffff;
  width: 60px;
  height: 60px;
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Impact, Garamond, Georgia, serif;
  font-size: 42pt;
  color: #666666;
  line-height: 60px;
  user-select: none;
  -moz-user-select: none;
  -o-user-select: none;
  -ms-user-select: none;
  border-top: 2px solid #eeeeee;
}

.t-bq-quote-emma .t-bq-quote-emma-qmark span {
  padding-top: 0.25em;
}

.t-bq-quote-emma .t-bq-quote-emma-userpic {
  flex-basis: 150px;
  width: 150px;
  min-width: 150px;
  max-height: auto;
  background: url("https://raw.githubusercontent.com/taviskaron/t-div-blockquotes/main/img/strug.jpg") center center no-repeat;
  background-size: cover;
  border-radius: 20px 0 0 20px;
}

.t-bq-quote-emma .t-bq-quote-emma-base {
  flex-basis: calc(100% - 150px);
  padding: 60px 30px 45px 30px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.t-bq-quote-emma .t-bq-quote-emma-base .t-bq-quote-emma-text {
  font-size: 16px;
  line-height: 30px;
}

.t-bq-quote-emma .t-bq-quote-emma-base .t-bq-quote-emma-text:after {
  content: "\2014\00A0" attr(cite);
  display: block;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  font-weight: bold;
  margin-top: 10px;
}

@media screen and (max-width: 768px) {

  .t-bq-quote-emma {
    flex-direction: column;
  }

  .t-bq-quote-emma .t-bq-quote-emma-base {
    padding-top: 0;
  }

  .t-bq-quote-emma .t-bq-quote-emma-userpic {
    border-radius: 20px;
    height: 150px;
    margin: 40px auto 20px auto;
  }

  .t-bq-quote-emma .t-bq-quote-emma-base .t-bq-quote-emma-text {
    font-size: 18px;
  }

main{
  height: 600px;
}
}



/* ========== 02. Sophia ========== */

.t-bq-quote-sophia .t-bq-quote-sophia-base {
  background: white;
  padding: 20px 40px 40px 40px;
  border-radius: 10px;
  margin-bottom: 40px;
  position: relative;
}

.t-bq-quote-sophia .t-bq-quote-sophia-base:after {
  content: "";
  position: absolute;
  background: #ffffff;
  transform: rotate(45deg);
  width: 30px;
  height: 30px;
  margin: 0 auto;
  bottom: -15px;
  left: calc(50% - 15px);
  z-index: -1;
}

.t-bq-quote-sophia .t-bq-quote-sophia-author {
  text-align: center;
  margin-bottom: 10px;
}

.t-bq-quote-sophia .t-bq-quote-sophia-text {
  font-size: 16px;
  line-height: 30px;
}

.t-bq-quote-sophia .t-bq-quote-sophia-author cite {
  font-style: normal;
  text-transform: uppercase;
  letter-spacing: 0.03em;
  font-size: 18px;
  font-weight: bold;
}

.t-bq-quote-sophia .t-bq-quote-sophia-userpic {
  width: 100px;
  height: 100px;
  background: url("https://raw.githubusercontent.com/taviskaron/t-div-blockquotes/main/img/strug.jpg") center center no-repeat;
  background-size: cover;
  margin: 0 auto;
  border-radius: 50%;
}









/* ========== 03. Jenny ========== */

.t-bq-quote-jenny .t-bq-quote-jenny-base {
  background: white;
  padding: 20px 40px 40px 40px;
  border-radius: 10px;
  margin-bottom: 40px;
  position: relative;
}

.t-bq-quote-jenny .t-bq-quote-jenny-base:after {
  content: "";
  position: absolute;
  background: #ffffff;
  transform: rotate(45deg);
  width: 30px;
  height: 30px;
  margin: 0 auto;
  bottom: -15px;
  left: calc(100% - 100px - 15px);
  z-index: -1;
}

.t-bq-quote-jenny .t-bq-quote-jenny-base .t-bq-quote-jenny-text {
  text-indent: 5em;
  line-height: 30px;
  font-size: 16px;
}

.t-bq-quote-jenny .t-bq-quote-jenny-base .t-bq-quote-jenny-text:before {
  content: "\201C";
  position: absolute;
  left: -55px;
  top: 55px;
  font-family: Georgia, serif;
  font-size: 160pt;
  color: #01A781FF;

}

.t-bq-quote-jenny .t-bq-quote-jenny-meta {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
}

.t-bq-quote-jenny .t-bq-quote-jenny-meta .t-bq-quote-jenny-meta-info {
  flex-basis: calc(100% - 50px);
}

.t-bq-quote-jenny .t-bq-quote-jenny-meta .t-bq-quote-jenny-author,
.t-bq-quote-jenny .t-bq-quote-jenny-meta .t-bq-quote-jenny-source {
  text-align: right;
  flex-basis: 100%;
  padding-right: 15px;
  line-height: 1.38em;
}

.t-bq-quote-jenny .t-bq-quote-jenny-meta .t-bq-quote-jenny-author cite {
  font-style: normal;
  text-transform: uppercase;
  letter-spacing: 0.03em;
  font-size: 10pt;
  font-weight: bold;
}

.t-bq-quote-jenny .t-bq-quote-jenny-meta .t-bq-quote-jenny-source span {
  font-size: 11pt;
}

.t-bq-quote-jenny .t-bq-quote-jenny-meta .t-bq-quote-jenny-userpic {
  flex-basis: 50px;
  flex-grow: 0;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin-left: auto;
}




</style>