<template>
  <div class="section-alpha">

    <p class="section-header-1">Trade with confidence</p>
    <p class="section-header">The numbers speak for themselves. Trade with the support of the world’s largest
      retail broker.</p>




    <div class="section-content">

      <div class="section-content-1" >
        <div class="box">
          <img src="https://www.bitfinex.com/images/features/features-more/pro_connectivity.svg" class="about-image" alt="assets-image"/>
          <h3>Professional connectivity</h3>
          <p>By collaborating with Market Synergy, corporate and professional traders can take advantage of the fastest
            trading speed through institutional-grade connectivity and co-location services, with direct access to our
            digital asset gateway.</p>
        </div>
        <div class="box">
          <img src="https://www.bitfinex.com/images/features/features-more/advanced_chart_features.svg" class="about-image" alt="assets-image"/>
          <h3>Advanced chart features</h3>
          <p>TopLeads Trade facilitates a graphical trading experience with advanced charting functionality that allows traders to visualise orders, positions and price alerts, tap to modify order properties, and annotate to their trading strategy.</p>
        </div>
        <div class="box">
          <img src="https://www.bitfinex.com/images/features/features-more/corp_accounts.svg" class="about-image" alt="assets-image"/>
          <h3>Corporate accounts</h3>
          <p>TopLeads Trade has a bespoke offering expertly tailored to meet the specific needs of professional and institutional traders including sub-accounts, expedited verification, and dedicated customer support.</p>
        </div>
      </div>

<!--      <div class="section-content-1" >-->
<!--        <div class="box">-->
<!--          <img src="https://margex.com/images/products_alerts.svg" class="about-image" alt="assets-image"/>-->
<!--          <h3>Price Alerts</h3>-->
<!--          <p>Stay in touch with all important market movements and price changes.</p>-->
<!--        </div>-->
<!--        <div class="box">-->
<!--          <img src="https://margex.com/images/products_crypto.svg" class="about-image" alt="assets-image"/>-->
<!--          <h3>Buy Crypto</h3>-->
<!--          <p>Purchase cryptocurrency through Early Wealth trusted partners.</p>-->
<!--        </div>-->
<!--        <div class="box">-->
<!--          <img src="https://margex.com/images/products_mobile.svg" class="about-image" alt="assets-image"/>-->
<!--          <h3>Two Mobile Apps</h3>-->
<!--          <p>"Early Wealth app" - For Traders "Copy trading app" - For Followers</p>-->
<!--        </div>-->
<!--      </div>-->


    </div>

  </div>
</template>

<script>
export default {
  name: "AboutSection3"
}
</script>

<style scoped>

.section-alpha{
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

.box{
  background-color: #ffffff;
  /*box-shadow:  20px 20px 60px #d9d9d9,*/
  /*-20px -20px 60px #ffffff;*/
  padding: 15px;
  border-radius: 5px;
  margin-bottom: 12px;
  margin-top: 4%;
  width: 350px;
  height: 400px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}



.section-content-1{
  display: flex;
  justify-content: space-evenly;
}

.about-image{
  display: block;
  margin-left: auto;
  margin-right: auto;
  height: 50px;
  width: 50px;
  object-fit: cover;
  margin-top: 7%;
}


.box h3{
  padding-top: 22px;
  color: #222222;
  font-weight: 500;
  text-align: center;
  margin-bottom: 6px;
}

.box p{
  color: #393939;
  text-align: center;
  font-size: 15px;
  line-height: 1.5;
  padding-top: 5%;
}


@media (max-width: 700px) {
  .section-header{
    font-size: 15px;
    margin-left: 10%;
    margin-right: 10%;
  }
  .section-content-1{
    display: flex;
    flex-direction: column-reverse;
    justify-content: space-evenly;
  }

  .section-header-1{
    font-size: 26px;
    width: 95%;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .box{
    /*margin-left: 10%;*/
    /*margin-right: 10%;*/
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
}



@media (max-width: 500px) {
  .section-header{
    margin-left: 4%;
    margin-right: 4%;
  }
}
</style>