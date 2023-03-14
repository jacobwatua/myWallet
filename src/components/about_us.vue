<template>
  <div class="about-us">
    <div class="about-header">
      About Us
    </div>
    <div class="logo">
      <img src="../assets/images/logo.png" alt="">
    </div>
    <div class="description">
      <p>
          <strong>Who are we?</strong><br/>
          We are a team of passionate professionals who believe in the power of data and 
          transparency to drive meaningful change in the business world. Our mission is to help businesses and 
          consumers make informed decisions by providing KPI-based rankings that are accurate, 
          reliable, and easy to understand. Our team consists of experienced analysts, data scientists, 
          and business experts who work tirelessly to collect, analyze, and verify data from various sources to 
          ensure that our rankings are up-to-date and unbiased. We use a rigorous methodology to ensure that our 
          rankings are based on the most relevant and meaningful KPIs for each industry, and that all businesses 
          are evaluated fairly and objectively. We are committed to providing a user-friendly and accessible platform 
          that is easy to navigate and provides valuable insights for our users. Whether you're a business owner looking 
          to improve your performance, or a consumer looking for the best options in your industry, we've got you covered.
          At myWallet, we are dedicated to providing the highest quality KPI-based rankings and to continuously improving 
          our platform to better serve our users. Thank you for visiting our site, and we hope you find our rankings helpful and informative.
      </p>
      <button class="btn btn-success">View Our Team</button>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
  .about-us {
    margin-top:  20px;
    display: grid;
    grid-template-columns: repeat(2, 50%);
    grid-auto-rows: 40px 1fr;
  }

  .about-header{
    grid-area: 1/1/2/2;
    display: flex;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    color: white;
    font-weight: bolder;
  }
  .description {
    color: lightcyan;
    grid-area: 1/2/3/3;
    box-sizing: border-box;
    padding: 20px;
    padding-top: 40px;
    text-align: justify;
  }
  .logo img {
    width: 100%;
    height: 100%;
    border-top-right-radius: 8px;
  }
</style>



