<template>

    <div class="alpha">



      <div class="header">
        <p class="text-1">Live cryptocurrency prices.</p>
        <p class="text-2">Get updated with the latest price movements for over 400 different spot markets.</p>
      </div>
      <div class="header-select">
        <p @click="changeScreen" class="btn">Cryptos</p>
        <p @click="changeScreen2" class="btn">Forex</p>
        <p @click="changeScreen3" class="btn">Stocks</p>
      </div>

      <crypto-table v-show="this.screen === 'crypto'"/>

      <forex-table v-show="this.screen === 'forex'"/>

      <stock-table v-show="this.screen === 'stocks'"/>


      <div class="section-2">
        <p class="text-5">Our numbers speak volumes</p>
        <p class="text-6">Volume data on TopLeads Trade’s state-of-the-art platform</p>

        <div class="separate">
          <div class="section-2-container">
            <p class="text-3">Past 24 Hours</p>
            <p class="text-4">$2,054m</p>
          </div>
          <div class="section-2-container">
            <p class="text-3">Past 7 Days</p>
            <p class="text-4">$14,625m</p>
          </div>
          <div class="section-2-container">
            <p class="text-3">Past 30 Days</p>
            <p class="text-4">$47,472m</p>
          </div>
        </div>

      </div>

    </div>

</template>

<script>
import CryptoTable from "@/components/BaseComponents/tables/CryptoTable.vue";
import ForexTable from "@/components/BaseComponents/tables/ForexTable.vue";
import StockTable from "@/components/BaseComponents/tables/StockTable.vue";

export default {
  name: "HomeSection4",
  components: {StockTable, ForexTable, CryptoTable},
  data() {
    return {
      screen: "crypto",
    };
  },
  methods: {
    changeScreen() {
      this.screen = "crypto"
    },
    changeScreen2() {
      this.screen = "forex"
    },
    changeScreen3() {
      this.screen = "stocks"
    },
  }
}
</script>

<style scoped>
/*.alpha{*/
/*  margin-top: 3%;*/
/*  margin-bottom: 5%;*/
/*}*/

.alpha{
  background-image: url("@/assets/manifesto-hero-bg.png");
  /*background-color: #000;*/
  height: 100%;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  padding-bottom: 5%;
  padding-top: 5%;
}

.header-select{
  display: flex;
  justify-content: center;
  gap: 15px;
  margin-bottom: 1%;
}

.btn{
  background: #01A781FF;
  border: 1px solid #01A781FF;
  color: #ffffff;
  padding: 0.6em 40px 0.5em 40px;
  border-radius: 6px;
  position: relative;
  display: inline-block;
  margin: 0;
  text-decoration: none;
  -webkit-transition: all 0.1s ease;
  transition: all 0.25s ease;
  margin-bottom: 1%;
}
.btn:hover{
  box-shadow: rgba(0, 0, 0, 0.35) 0px 3px 13px;
}

.text-1{
  font-size: 28px;
  text-align: center;
  color: #071333;
  padding-bottom: 15px;
  font-weight: 700;
}

.text-2{
  font-size: 18px;
  text-align: center;
  color: #0f171c;
  margin-bottom: 2%;
}

.text-3{
  font-size: 18px;
  text-align: center;
  color: #ffffff;
  margin-bottom: 3%;
}

.text-4{
  font-size: 38px;
  text-align: center;
  color: rgba(3, 202, 155, 100);
  margin-bottom: 2%;
}

.text-5{
  font-size: 28px;
  text-align: left;
  color: #071333;
  padding-bottom: 15px;
  font-weight: 700;
}

.text-6{
  font-size: 18px;
  text-align: left;
  color: #0f171c;
  margin-bottom: 2%;
}

.header{
  width: 60%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 2%;
}

.section-2{
  margin-left: 5%;
  margin-bottom: 4%;
  margin-top: 5%;
}

.section-2-container{
  -webkit-backdrop-filter: blur(5px);
  backdrop-filter: blur(5px);
  background: rgba(17, 42, 63, .8);
  border-radius: 6px;
  display: inline-block;
  padding: 15px 100px;
  box-shadow: rgba(0, 0, 0, 0.3) 0px 3px 13px;
  margin-top: 5px;
}

.separate{
  display: flex;
  gap: 20px;
  justify-content: center;
}

@media (max-width: 990px) {

}

@media (max-width: 700px){

  .header{
    width: 95%;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .text-1{
    font-size: 24px;
    padding-bottom: 20px;
  }

  .text-2{
    font-size: 16px;
  }

  .header-select{
    gap: 5px;
    margin-top: 3%;
    margin-bottom: 5%;
  }

  .btn{
    padding: 0.5em 30px 0.4em 30px;
  }

}

@media (max-width: 500px){

}

</style>