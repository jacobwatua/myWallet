<template>
  <div class="content-card">
    <div class="box box1">
      <h1 class="text-center">Welcome to<br>myWallet</h1>
    </div>
    <div class="box box2">
      <p class="tex-center">
        This is where the best businesses rise to the top! We're your go-to destination
        for finding the top performers in your industry based on the metrics that matter most. Whether you're looking for
        the most efficient operations, highest customer satisfaction, or greatest revenue growth, we've got you covered.
        So come on in, explore our rankings, and discover the businesses that are leading the way!
      </p>
      <button class="btn btn-danger">Learn More</button>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .content-card{
        background-color: #004242;
        width: 100%;
        height: 60vh;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        color: white;
        margin-top: 70px;
    }
    .box {
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .box2{
      padding: 30px;
      color: lightblue;
      text-align: justify;
      flex-direction: column;
    }
</style>
