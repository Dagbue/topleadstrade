<template>
  <div class="alpha">

    <div class="section-alpha">

      <img src="https://www.bitfinex.com/images/features/parallax-coins/coin-1.svg" alt="" class="hero-section-image-1"/>
      <img src="https://www.bitfinex.com/images/features/parallax-coins/coin-2.svg" alt="" class="hero-section-image-2"/>
      <img src="https://www.bitfinex.com/images/features/parallax-coins/coin-3.svg" alt="" class="hero-section-image-3"/>


      <div class="section-1">
        <p class="text-1">World class <span style="color: #01A781FF">Trading features<br/> </span> Through Advanced Strategies</p>


        <p class="text-2">Order Trades with top tier liquidity so you can take advantage of every situation
          <br/> Your assets, your choices, our technology. Empowering your financial freedom.
        </p>

        <img src="https://www.bitfinex.com/images/mobile-app-screens.png" alt="" class="image-lst"/>

<!--        <div class="button-group">-->
<!--          <div class="btn-1" @click="onPostClick">-->
<!--            Get Started-->
<!--            &lt;!&ndash;            <img src="@/assets/arrow-right-line.svg" alt="" class="" />&ndash;&gt;-->
<!--          </div>-->
<!--          <div class="btn-1" @click="onPostClick2">-->
<!--            LogIn-->
<!--            &lt;!&ndash;            <img src="@/assets/arrow-right-line.svg" alt="" class="" />&ndash;&gt;-->
<!--          </div>-->
<!--        </div>-->
      </div>

<!--      <div class="section-2">-->
<!--        <img src="@/assets/iphonex.png" alt="" class="image" />-->
<!--        &lt;!&ndash;        <video autoplay="" muted="" loop="">&ndash;&gt;-->
<!--        &lt;!&ndash;          <source src="https://margex.com/videos/header_mobile_video.mp4" type="video/mp4">&ndash;&gt;-->
<!--        &lt;!&ndash;        </video>&ndash;&gt;-->
<!--      </div>-->

      <img src="https://www.bitfinex.com/images/features/parallax-coins/coin-4.svg" alt="" class="hero-section-image-4"/>
      <img src="https://www.bitfinex.com/images/features/parallax-coins/coin-5.svg" alt="" class="hero-section-image-5"/>
      <img src="https://www.bitfinex.com/images/features/parallax-coins/coin-6.svg" alt="" class="hero-section-image-6"/>


    </div>


  </div>
</template>

<script>
export default {
  name: "AboutSectioon1",
  data() {
    return {
      currentIndex: 0,
      items: [
        { name: 'Forex', color: '#009688' },  // Red
        { name: 'RealEstate', color: '#984613' }  ,  // Yellow
        { name: 'Crypto', color: '#3071EE' }, // Green
        { name: 'Stocks', color: '#5d78ff' }, // Blue
        { name: 'CFD', color: '#fe9431' }    // Yellow
      ],
      intervalId: null
    };
  },
  mounted() {
    this.startRotation();
  },
  beforeDestroy() {
    clearInterval(this.intervalId);
  },
  methods: {
    startRotation() {
      this.intervalId = setInterval(() => {
        this.currentIndex = (this.currentIndex + 1) % this.items.length;
      }, 2000); // Change item every 2000 milliseconds
    },
    onPostClick() {
      this.$router.push("/register");
    },
    onPostClick2() {
      this.$router.push("/login");
    },
  }
}
</script>

<style scoped>
.section-alpha{
  background-color: #0d1d29;
  height: 600px;
  position: relative;
}
.hero-section-image-1{
  position: absolute;
  top: 100px;
  left: 130px;
}
.hero-section-image-2{
  position: absolute;
  top: 245px;
  left: 60px;
}
.hero-section-image-3{
  position: absolute;
  top: 435px;
  left: 115px;
}

.hero-section-image-4{
  position: absolute;
  top: 100px;
  left: 1200px;
  right: 0;
}
.hero-section-image-5{
  position: absolute;
  top: 260px;
  left: 1250px;
  right: 0;
}
.hero-section-image-6{
  position: absolute;
  top: 435px;
  left: 1210px;
  right: 0;
}
.items-switch .active {
  display: inline; /* Show only active item */
}
.items-switch .active {
  display: inline; /* Show only active item */
}

.items-switch span {
  display: none; /* Hide all by default */
}
.section-alpha{
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  /*flex-direction: column;*/
}

.section-1{
  /*margin-top: 50px;*/
}

.section-2{
  /*margin-bottom: -10px;
  width: 255px;
  height: 500px;
  background: url("https://margex.com/images/phone_border.svg");
  background-repeat: no-repeat;
  -webkit-background-position: center;
  background-position: center;
  -webkit-background-size: contain;
  background-size: contain;
  padding: 12px 16px 0;*/
}

video{
  width: 100%;
  border-radius: 30px;
}
.text-1{
  font-size: 44px;
  line-height: 64px;
  letter-spacing: -0.01em;
  text-align: center;
  margin-bottom: 8px;
  color: #FFFFFF;
  font-weight: 700;
}

.text-2{
  font-size: 18px;
  line-height: 24px;
  letter-spacing: -0.015em;
  text-align: center;
  color: #7A849D;
}

.btn-1{
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  height: 46px;
  padding: 8px 16px;
  border-radius: 12px;
  gap: 8px;
  background: #01A781FF;
  border: 1px solid #01A781FF;
  width: 160px;
  /*margin-left: auto;*/
  /*margin-right: auto;*/
  color: #FFFFFF;
  /*margin-bottom: 30px;*/
}

.image{
  width: 55%;
  display: block;
  /*margin-left: auto;*/
  margin-right: auto;
  margin-left: 35%;
}


.button-group{
  display: flex;
  justify-content: left;
  gap: 10px;
}

.image-lst{
  width: 30%;
  display: block;
  margin-right: auto;
  margin-left: auto;
  margin-top: 2%;
}

@media (max-width: 990px) {

}

@media (max-width: 700px) {

  .hero-section-image-1{
    display: none;
  }
  .hero-section-image-2{
    display: none;
  }
  .hero-section-image-3{
    display: none;
  }

  .hero-section-image-4{
    display: none;
  }
  .hero-section-image-5{
    display: none;
  }
  .hero-section-image-6{
    display: none;
  }

  .section-alpha{
    height: 100%;
    padding-top: 5%;
    padding-bottom: 5%;
  }

  .section-alpha{
    display: block;
  }

  .section-1{
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .text-1{
    font-size: 40px;
    line-height: 45px;
    margin-bottom: 8px;
    /*width: 90%;*/
    /*margin-left: auto;*/
    /*margin-right: auto;*/
    text-align: center;
  }

  .text-2{
    font-size: 15px;
    line-height: 20px;
    text-align: center;
  }

  .btn-1{
    height: 40px;
    padding: 8px 16px;
    gap: 6px;
    width: 160px;
    font-size: 14px;
  }

  .button-group{
    display: flex;
    justify-content: center;
    gap: 12px;
  }

  .section-2{
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-top: 5%;
  }

  video{
    width: 100%;
    border-radius: 30px;
  }

  .image-lst{
    width: 70%;
  }
}

@media (max-width: 500px) {
  .text-1{
    font-size: 35px;
    line-height: 40px;
    margin-bottom: 9px;
  }



  .text-2{
    width: 85%;
    margin-left: auto;
    margin-right: auto;
  }
}
</style>