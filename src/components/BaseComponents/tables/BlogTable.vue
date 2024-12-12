<template>
  <div class="tradingview-widget-container">

    <div class="header">
      <p class="text-1">Latest news.</p>
      <p class="text-2">Get the latest market news, trading analysis, and feature updates.</p>
    </div>

    <div id="tradingview-widget" class="tradingview-widget"></div>
  </div>
</template>
<script>
export default {
  name: "BlogTable",
  mounted() {
    this.loadTradingViewScript();
  },
  methods: {
    loadTradingViewScript() {
      const script = document.createElement('script');
      script.src = 'https://s3.tradingview.com/external-embedding/embed-widget-timeline.js';
      script.async = true;
      script.innerHTML = JSON.stringify({
        "feedMode": "all_symbols",
        "isTransparent": false,
        "largeChartUrl": "http://www.assettrademarkets.com",
        "displayMode": "regular",
        "width": "100%",
        "height": "100%",
        "colorTheme": "light",
        "locale": "en"
      });

      document.getElementById('tradingview-widget').appendChild(script);
    }
  }
}
</script>

<style scoped>
.tradingview-widget-container{
  padding-top: 5%;
  padding-bottom: 5%;

  background-image: url("@/assets/manifesto-hero-bg.png");
  /*background-color: #000;*/
  height: 100%;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.tradingview-widget {
  width: 96%; /* Adjust width as needed */
  height: 700px; /* Adjust height as needed */
  display: block;
  margin-right: auto;
  margin-left: auto;
}


.text-1{
  font-size: 28px;
  text-align: center;
  color: #071333;
  padding-bottom: 5px;
  font-weight: 700;
}

.text-2{
  font-size: 18px;
  text-align: center;
  color: #0f171c;
  margin-bottom: 3%;
}

.header{
  width: 60%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>