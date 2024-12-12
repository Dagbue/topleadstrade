<template>
  <div class="alpha">
    <p class="section-header-1">Focus on trading. We’ll handle the rest.</p>
    <p class="section-header">You decide what to trade and when to trade it. We’re hard at work behind the scenes to
      minimize your costs and improve your execution.</p>


    <div class="section-alpha">

      <div class="section-2">

        <img src="https://www.bitfinex.com/images/features/features-list/margin_funding.svg" alt="image" class="image" />

      </div>


      <div class="section-1">

        <div class="text-part">
          <p class="text-1">Margin funding</p>
          <p class="text-2">
            Our margin funding market allows you to earn interest on fiat and digital assets by providing funding to
            traders wanting to trade with leverage. You can offer funding across a wide range of currencies & assets,
            at the rate and duration of your choice and use TopLeads Trade Lending Pro to automate your lending based on your
            preferences.
          </p>
        </div>

<!--        <div class="text-part">-->
<!--          <p class="text-1">No market impact</p>-->
<!--          <p class="text-2">Trade large orders with the same spread and pricing as any other trader.</p>-->
<!--        </div>-->

<!--        <div class="text-part">-->
<!--          <p class="text-1">Better trade implementation</p>-->
<!--          <p class="text-2">Benefit from our proprietary trade implementation process with guaranteed liquidity.</p>-->
<!--        </div>-->


      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: "AboutSection5"
}
</script>

<style scoped>

.alpha{
  background-image: url("@/assets/leaf-bg.svg");
  /*background-color: #000;*/
  height: 100%;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  padding-bottom: 5%;
  padding-top: 5%;
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
  width: 80%;
  display: block;
  margin-right: auto;
  margin-left: auto;
  margin-bottom: 3%;
}

.text-1{
  font-size: 28px;
  line-height: 26px;
  font-weight: 700;
  white-space: pre-line;
  margin-bottom: 10px;
  color: #0f171c;
}

.text-2{
  margin: 0;
  color: #222222;
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
  }
  .section-alpha{
    display: block;
  }
  .section-1{
    width: 100%;
  }

  .section-2{
    width: 100%;
    margin-bottom: 5%;
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
    width: 55%;
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