<template>
  <div class="alpha">

    <div class="header">
      <h2 class="text-1">Features of Topleads Trade</h2>
    </div>

    <div class="section-alpha">

      <div class="section-1">
        <div class="section-1-inner">
          <h2 class="text-2">A Personal Trading Strategist</h2>
          <p class="text-3">
            Collaborate closely with your dedicated advisor to gain clarity on your financial objectives, evaluate
            the full spectrum of your investment opportunities, and develop a personalized trading strategy that not
            only aligns with your unique goals but also adapts to changing market conditions. Together, you’ll craft
            a plan that positions you for long-term success and growth.
          </p>
        </div>
      </div>

      <div class="section-2">
        <img src="@/assets/mission.svg" alt="" class="image"/>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: "FeaturesPart"
}
</script>

<style scoped>
.alpha{
  padding-top: 5%;
  padding-bottom: 5%;
  background: #f4f5f6;
}

.text-1{
  text-align: center;
  font-size: 28px;
  font-weight: 700;
}

.section-1{
  width: 55%;
}
.section-2{
  width: 45%;
}

.section-1-inner{
  width: 70%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.section-alpha{
  display: flex;
  align-items: center;
  align-content: center;
  padding-top: 3%;
}

.image{
  width: 95%;
  background-color: #0d1d29;
}

.text-2{
  padding-bottom: 10px;
  font-size: 30px;
  color: #0f171c;
  font-weight: 700;
}

.text-3{
  line-height: 1.4;
  width: 80%;
  /*color: #667085;*/
}

@media (max-width: 990px) {

}

@media (max-width: 700px){
  .section-alpha{
    display: block;
  }

  .image{
    width: 90%;
    display: block;
    margin-right: auto;
    margin-left: auto;
    margin-top: 5%;
  }

  .text-2{
    font-size: 25px;
    text-align: center;
  }

  .section-1-inner{
    width: 90%;
  }

  .alpha{
    padding-top: 10%;
    padding-bottom: 15%;
  }
  .section-1{
    width: 100%;
  }
  .section-2{
    width: 100%;
  }
  .text-3{
    line-height: 1.4;
    width: 100%;
    /*color: #667085;*/
  }
}

@media (max-width: 500px){

}
</style>