<template>
  <div class="alpha-2">
    <div class="section-1">
      <p class="last-text">Start trading today</p>
      <div class="seperate mobile">
        <p class="download-sub"><a
            style="color: #000000;"
            href="mailto:support@topleadstrd.com">support@topleadstrd.com</a></p>
      </div>
      <div class="seperate mobile">
        <p class="download-sub">45 Green Lane, London, United Kingdom, EC1V 1AA.</p>
      </div>

      <div class="button-seprate" @click="onPostClick">
        <button class="button">
          Contact Us
          <img src="@/assets/arrow-right-line.svg" alt="btn-image" class="btn-image" />
        </button>

<!--        <button class="button">-->
<!--          Contact Us-->
<!--          <img src="@/assets/arrow-right-line.svg" alt="btn-image" class="btn-image" />-->
<!--        </button>-->
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "ReadyToWork",
  methods: {
    onPostClick() {
      this.$router.push("/contact");
      window.scrollTo(0, 0);
    },
  },
}
</script>

<style scoped>
.alpha-2{
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 1000px;
  height: 270px;
  border-radius: 16px;
  margin-top: 4%;
  margin-bottom: 5%;

  /*width: 11522px;*/
  /*height: 100%;*/
  background: url("@/assets/background1.png") repeat-x;
  background-color: #f4f4f5;
  -webkit-background-size: contain;
  background-size: cover;
  /*position: absolute;*/
  /*top: 0;*/
  /*left: 0;*/
  /*-webkit-animation: bg-slide 60s linear infinite;*/
  /*animation: bg-slide 60s linear infinite;*/
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}

/*@keyframes bg-slide {*/
/*  0% {*/
/*    transform: translateZ(0);*/
/*  }*/
/*  100% {*/
/*    transform: translate3d(-3840px, 0, 0);*/
/*  }*/
/*}*/


.section-1{
  text-align: center;
}

.last-text{
  color: #101828;
  font-size: 30px;
  line-height: 44px;
  padding-top: 5%;
  padding-bottom: 0.5%;
  font-weight: 700;
}

.button {
  background: #01A781FF;
  border: 1px solid #01A781FF;
  color: white;
  cursor: pointer;
  padding: 12px 40px;
  text-align: center;
  border-radius: 12px;
  display: flex;
  align-content: center;
  align-items: center;
  justify-content: center;
  gap: 2.5px;
  font-size: 15px;
}

button{
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 10px;
}

/*.button:hover {*/
/*  background: #070e20;*/
/*  border: solid 1px #070e20;*/
/*}*/

.btn-image{
  width: 15%;
}


.seperate{
  display: flex;
  align-content: center;
  align-items: center;
}

i{
  padding-top: 1.5%;
  font-size: 25px;
  color: #000000;
}

.download-sub{
  color: #000000;
  font-size:18px;
  line-height: 28px;
  width: 75%;
  display: block;
  margin-right: auto;
  margin-left: auto;
  padding-bottom: 10px;
}
/*.button-seprate{*/
/*  display: flex;*/
/*  justify-content: center;*/
/*  gap: 15px;*/
/*  margin-top: 10px;*/
/*}*/

@media (max-width: 700px){
  .alpha-2{
    width: 650px;
    margin-top: 5%;
  }

  .last-text{
    padding-top: 8%;
  }
}

@media (max-width: 500px){

  .alpha-2{
    width: 400px;
    margin-top: 5%;
  }

  .download-sub{
    font-size: 16px;
    width: 100%;
  }

  .last-text{
    font-size: 27px;
  }

}
</style>