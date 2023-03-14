<template>
  <div class="vision-mission">

    <div class="vision">
        <p class="text-center">Our Vision</p>
        <p class="">To become the ultimate destination for businesses and consumers alike,
          by providing transparent and accurate KPI-based rankings, empowering informed decision-making.
        </p>
    </div>

    <div class="mission">
      <p class="text-center">Our Mission</p>
      <p class="">
        At myWallet, our mission is to help businesses improve their performance by providing
        actionable insights and benchmarks, while at the same time helping consumers find the best 
        businesses based on KPIs that matter most to them. We strive to be the most comprehensive and 
        trusted source for KPI-based rankings, and to continuously innovate and improve our platform to better serve our users.
      </p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .vision-mission {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        background-color: #1b1b1b;
        color: #f6f7f8;
        padding: 30px;
        font-size: 15px;
        margin: 20px 0px;
    }

    .vision-mission div {
      padding: 20px;
      box-sizing: border-box;
    }
</style>