<template>
  <div class="alpha">

    <div class="section-1">
      <h2 class="text-1" style="text-align: center;"> TopLead Trade is More than Just a Trading Platform</h2>
      <p class="text-2">Give your trading strategy the advantage with our better-than-market conditions.</p>
    </div>


    <div  class="section-1-inner">

      <div class="section-1-inner-content">
        <img src="@/assets/trend-up.svg" alt="" class="image"/>
        <br/>
        <h1>Spot trading</h1>
        <p class="description">
          Trade Bitcoin, Ethereum, Solana and other cryptocurrencies with minimal slippage, tight pricing and optimize
          your performance. TopLead Trade offers order books with top tier liquidity with a suite of different order types.
        </p>
      </div>

      <div class="section-1-inner-content">
        <img src="@/assets/candle-chart.svg" alt="" class="image"/>
        <br/>
        <h1>Margin trading</h1>
        <p class="description">
          Trade with up to 10x leverage using TopLead Trade’s margin trading. You can enter an order for your desired
          funding amount, rate and duration, or simply open a position. Let us take care of the rest.
        </p>
      </div>

      <div class="section-1-inner-content">
        <img src="@/assets/fork.svg" alt="" class="image"/>
        <br/>
        <h1>Stake and earn</h1>
        <p class="description">
          Hold your digital tokens and generate rewards of up to 7% per year with the TopLead Trade staking programme.
        </p>
      </div>

    </div>

    <div class="btn-part">
      <div class="btn-1" @click="onPostClick">Create Account</div>
      <p class="btn-2" @click="onPostClick2">Log In</p>
    </div>


  </div>
</template>

<script>
export default {
  name: "HomeSection2",
  methods: {
    onPostClick() {
      this.$router.push("/register");
    },
    onPostClick2() {
      this.$router.push("/login");
    },
  },
}
</script>

<style scoped>

.alpha{
  padding-top: 5%;
  padding-bottom: 5%;
  /*background: #f4f5f6;*/

  background-image: url("@/assets/leaf-bg.svg");
  /*background-color: #000;*/
  height: 100%;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.section-1-inner{
  display: flex;
  margin-top: 4%;
}

.section-1-inner-content{
  text-align: center;
  width: 46%;
}
.section-1-inner-content h1{
  font-size: 19px;
  padding-bottom: 5px;
  font-weight: 700;
}

.description{
  width: 75%;
  font-size: 15px;
  line-height: 1.5;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.description-2{
  width: 55%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.image{
  display: block;
  margin-left: auto;
  margin-right: auto;
  object-fit: cover;
  width: 65px;
}

.image-2{
  display: block;
  margin-left: auto;
  margin-right: auto;
  object-fit: cover;
  width: 65px;
}

.text-1{
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 30%;
  font-size: 24px;
  padding-bottom: 10px;
  font-family: 'BR-Firma-Bold', sans-serif;
}
.text-2{
  font-size: 18px;
  text-align: center;
  padding-bottom: 1%;
}
.bx{
  font-size: 30px;
  margin-top: 10px;
}

.image-part{
  display: flex;
  justify-content: center;
  margin-top: 15px;
  gap: 20px;
}

.btn-part{
  display: flex;
  justify-content: center;
  gap: 15px;
  margin-top: 3%;
}

.btn-1{
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  height: 48px;
  padding: 8px 16px;
  border-radius: 14px;
  gap: 8px;
  background-color: transparent;
  border: 1px solid #01A781FF;
  color: #01A781FF;
  width: 180px;
}

.btn-2{
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  height: 48px;
  padding: 8px 16px;
  border-radius: 14px;
  gap: 8px;
  background: #01A781FF;
  border: 1px solid #01A781FF;
  width: 180px;
  color: #ffffff;
}


@media (max-width: 990px){

  .image{
    width: 60%;
    display: block;
    margin-right: auto;
    margin-left: auto;
    margin-top: 3%;
  }


  .alpha{
    padding-top: 10%;
    padding-bottom: 10%;
  }

  .text-1{
    width: 90%;
  }

  .section-1-inner{
    display: block;
  }

  .image{
    display: block;
    margin-left: auto;
    margin-right: auto;
    object-fit: cover;
    width: 180px;
  }

  .section-1-inner-content{
    text-align: center;
    width: 100%;
  }

  .btn-part{
    margin-top: 5%;
  }

}

@media (max-width: 500px){

  .section-1-inner{
    display: block;
  }

  .image{
    display: block;
    margin-left: auto;
    margin-right: auto;
    object-fit: cover;
    width: 100px;
  }



  .text-2{
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 90%;
  }
}
</style>