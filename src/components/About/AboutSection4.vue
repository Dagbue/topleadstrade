<template>
  <div class="alpha">
    <p class="section-header-1">Trading with Confidence and Security.</p>
    <p class="section-header">Experience Transparent Practices, Reliable Regulation, and Safeguarded Funds with Us.</p>


    <div class="section-alpha">

      <div class="section-1">

        <div class="text-part">
          <p class="text-1">Margin trading</p>
          <p class="text-2">Trade with up to 10x leverage with funding
            from our peer to peer margin funding platform. You can enter an order to borrow the desired amount
            at the rate and duration of your choice, or you can simply open a position and TopLeads Trade will take out
            funding for you at the best available rate at that time.</p>
        </div>

<!--        <div class="text-part">-->
<!--          <p class="text-1">Multiple regulatory licenses</p>-->
<!--          <p class="text-2">We are licensed and regulated by leading international governing bodies. Trade knowing-->
<!--            your financial data is protected.</p>-->
<!--        </div>-->

<!--        <div class="text-part">-->
<!--          <p class="text-1">Segregated accounts</p>-->
<!--          <p class="text-2">Your funds are always kept separate from company funds, so you’ll always have access to-->
<!--            them. No ifs, no buts.</p>-->
<!--        </div>-->


      </div>

      <div class="section-2">

        <img src="https://www.bitfinex.com/images/features/features-list/margin_trading.svg" alt="image" class="image" />

      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: "AboutSection4"
}
</script>

<style scoped>
/*.alpha{*/
/*  !*background-color: #f0f2f4;*!*/
/*  padding-bottom: 3%;*/
/*  padding-top: 3%;*/
/*}*/
.alpha{
  padding-top: 5%;
  padding-bottom: 5%;
  background: #f4f5f6;
}

.section-1{
  width: 50%;
}

.section-2{
  width: 50%;
}

.section-header{
  font-size: 17px;
  color: #0f171c;
  text-align: center;
  font-weight: 300;
  margin-left: 23%;
  margin-right: 23%;
  padding-bottom: 1%;
}
.section-header-1{
  font-size: 30px;
  color: #222222;
  font-weight: 700;
  text-align: center;
  padding-bottom: 0.5%;
  width: 42%;
  display: block;
  margin-right: auto;
  margin-left: auto;
}
.section-alpha{
  display: flex;
  justify-content: space-around;
  align-items: center;
  align-content: center;
  margin-top: 3%;
}

.image{
  width: 50%;
  display: block;
  margin-right: auto;
  margin-left: auto;
  align-items: center;
  border: 1px solid #2a3f4d;
  background-color: #2a3f4d;
  border-radius: 10px;
  justify-content: center;
  position: relative;
  padding: 60px 40px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}

.text-part{
  width: 75%;
  display: block;
  margin-right: auto;
  margin-left: auto;
  margin-bottom: 5%;
}

.text-1{
  font-size: 28px;
  line-height: 26px;
  font-weight: 700;
  white-space: pre-line;
  margin-bottom: 10px;
}

.text-2{
  margin: 0;
  font-size: 17px;
  white-space: pre-line;
  line-height: 1.4;
}

@media (max-width: 700px) {
  .section-header{
    font-size: 16px;
    margin-left: 8%;
    margin-right: 8%;
  }
  .section-header-1{
    font-size: 28px;
    width: 85%;
    display: block;
    margin-right: auto;
    margin-left: auto;
  }
  .section-alpha{
    display: block;
  }
  .section-1{
    width: 100%;
  }

  .section-2{
    width: 100%;
  }

  .text-1{
    font-size: 26px;
    line-height: 24px;
    margin-bottom: 13px;
  }

  .text-2{
    font-size: 16px;
    line-height: 1.3;
  }
  .image{
    width: 90%;
  }
}


@media (max-width: 500px) {

  .text-part{
    width: 85%;
  }
  .section-header-1{
    width: 90%;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

}
</style>