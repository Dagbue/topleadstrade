<template>
  <div class="alpha">
    <p class="section-header-1">Open an account and start trading commodities</p>
    <p class="section-header">Your funds and data are always secure. With Early Wealth you’re protected
      by industry-leading protocols.</p>


    <div class="section-alpha">

      <div class="section-1">

        <div class="text-part">
          <p class="text-1">Derivatives For advanced traders.</p>
          <p class="text-2">
            Advanced traders can use the TopLeads Trade Derivatives to trade perpetual futures, which enable traders to
            speculate on the future price of an asset. Further Derivative Products are on the way. TopLeads Trade
            Derivatives is provided by iFinex Financial Technologies Limited.
          </p>
        </div>

<!--        <div class="text-part">-->
<!--          <p class="text-1">Trade some of the most popular commodities online</p>-->
<!--          <p class="text-2">including gold and crude oil with both low and stable spreads.</p>-->
<!--        </div>-->

<!--        <div class="text-part">-->
<!--          <p class="text-1">Leverage unique trading conditions</p>-->
<!--          <p class="text-2">like Stop Out Protection to give your strategy an advantage.</p>-->
<!--        </div>-->


      </div>

      <div class="section-2">

        <img src="https://www.bitfinex.com/images/features/features-list/derivatives.svg" alt="image" class="image" />

      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: "AboutSection6"
}
</script>

<style scoped>
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
    width: 90%;
    display: block;
    margin-left: auto;
    margin-right: auto;
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